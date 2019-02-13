<template>
  <div class="about">
    <h1>This is an about page</h1>
    <Todo/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Todo from "@/components/Todo.vue";

@Component({
  components: {
    Todo
  }
})
export default class About extends Vue {}
</script>

<style scoped lang="scss">
</style>
