<template>
  <button @click="onClick()" :style="{ background: color }">Add task</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
      onClick() {
        console.log('yoou clicked');

      }
  }
};
</script>

