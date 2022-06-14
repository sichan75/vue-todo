<template>
  <div class="app__wrapper">
    <div>
      <div v-for="item in items" v-bind:key="item">
        <TodoItem :title="item" />
      </div>
    </div>
  </div>
</template>

<script>
import TodoItem from "./components/TodoItem.vue";

const items = () => ["아이템1", "아이템2"];

export default {
  name: "App",
  components: {
    TodoItem,
  },
  data() {
    return {
      items: items(),
    };
  },
};
</script>

<style>
.app__wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
