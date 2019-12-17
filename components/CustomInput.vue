<template>
  <v-text-field
    v-bind:value="value"
    v-on:input="$emit('input', value)"
  />
</template>

<script>
export default {
  name: 'CustomInput',
  props: {
    value: {
      type: String,
      required: true
    }
  },
  watch: {
    value () {
      this.$emit('input', this.value)
      console.log(this.value)
      console.log('Hello')
    }
  }
}
</script>
