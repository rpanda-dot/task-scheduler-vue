<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green" />
  </header>
</template>
<script>
import Button from "./Button";

export default {
  name: "Header",
  props: {
    title: {
      type: String,
      default: "My Title",
    },
    // Other ways to define props
    // props: ["title"],
    // props: {
    //   title: String,
    // },
  },
  components: { Button },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>