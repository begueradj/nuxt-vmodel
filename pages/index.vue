<template>
  <div>
    <custom-input v-model="value" />
    <v-btn @click="onClickChild">
      Ok
    </v-btn>
  </div>
</template>

<script>
import CustomInput from '@/components/CustomInput.vue'
export default {
  components: { CustomInput },
  data () {
    return {
      value: 'hello'
    }
  },
  /* watch: {
    value (val) {
      console.log('value: ' + val)
    }
  }, */
  methods: {
    showValue () {
      console.log('value is: ' + this.value)
    },
    onClickChild () {
      console.log(this.value) // someValue
    }
  }
}
</script>
