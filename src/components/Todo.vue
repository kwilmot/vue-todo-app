<template>
  <section>
    <h1>This is a todo!</h1>
    <h1>cookie: {{ cookie }}</h1>
  </section>
</template>

<script lang="ts">
import { Component, Vue, Prop } from "vue-property-decorator";

@Component
export default class Todo extends Vue {
  // public cookie: any = document.cookie;
  // public logCookie() {
  //   console.log(this.cookie);
  // }
  @Prop() private cookie: any = JSON.stringify(document.cookie);
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
