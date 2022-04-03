<template>
  <button @click="onClick" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "MyButton",
  props: {
    text: {
      type: String,
      default: "Add",
    },
    color: String,
  },

  methods: {
    onClick() {
      this.$emit('btn-click')
    },
  },
};
</script>
