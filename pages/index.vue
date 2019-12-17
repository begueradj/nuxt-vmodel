<template>
  <custom-input v-model="value" />
</template>

<script>
import CustomInput from '@/components/CustomInput.vue'
export default {
  components: { CustomInput },
  data () {
    return {
      value: ''
    }
  }
}
</script>
