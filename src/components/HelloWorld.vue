<template>
  <div class="content-block">
    <input
    :value="modelValue"
    @input="$emit('update:modelValue', $event.target.value)"
  />
  </div>
</template>
<script>
export default {
  props: {
    modelValue: String
  },
  emits: ['update:modelValue']
}
</script>
