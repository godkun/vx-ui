<template functional>
  <option :disabled="props.disabled" :value="props.value" :label="props.label"><slot></slot></option>
</template>
<script>
export default {
  componentName: 'XOption',
  props: {
    value: {
      type: String
    },
    disabled: {
      type: Boolean,
      default: false
    },
    label: {
      type: String
    }
  }
}
</script>
