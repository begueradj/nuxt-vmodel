<template>
  <v-text-field
    v-bind:value="ok"
    v-on:input="$emit('input', $event)"
  />
</template>

<script>
export default {
  name: 'CustomInput',
  model: {
    prop: 'ok',
    event: 'input'
  },
  props: {
    ok: {
      type: String,
      default: ''
    }
  }
  /* watch: {
    value () {
      this.$emit('input', this.value)
      console.log(this.value)
      console.log('Hello')
    }
  } */
}
</script>
