<template>
  <div class="wrapper">
    <p>{{ title }}</p>
  </div>
</template>

<script>
export default {
  name: "TodoItem",
  props: {
    title: String,
  },
};
</script>

<style>
.wrapper {
  max-width: 500px;
  width: 100%;
  padding: 5px 12px;
  border: 1px solid black;
}
p {
  margin: 0;
}
</style>
