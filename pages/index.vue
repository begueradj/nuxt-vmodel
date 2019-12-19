<template>
  <div>
    <custom-input v-model="bill" />
    <v-btn @click="clickChild">
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
      bill: 'moi'
    }
  },
  /* watch: {
    value (val) {
      console.log('value: ' + val)
    }
  }, */
  methods: {
    clickChild () {
      console.log('value is: ' + this.bill)
    }
  }
}
</script>
