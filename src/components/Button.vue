<template>
  <button @click="handleClick">
    {{ text }}
  </button>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true
    }
  },
  methods: {
    handleClick() {
      this.$emit("click");
    }
  }
};
</script>