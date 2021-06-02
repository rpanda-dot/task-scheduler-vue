<template>
  <button v-on:click="onClick()" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
      default: "New Button",
    },
    color: {
      type: String,
      default: "blue",
    },
  },
  methods: {
    onClick() {
      console.log("button clicked");
    },
  },
  //   props: ["text", "color"],
};
</script>