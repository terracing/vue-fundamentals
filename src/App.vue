<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <div>
    <h1>{{ text }}</h1>
    <p>{{ another }}</p>
  </div>
</template>

<script>
import base from "@/mixins/base";

export default {
  name: "App",
  mixins: [base],
  data() {
    return {
      text: "Hello Vue!",
    };
  },
  beforeCreate() {
    console.log("beforeCreate", this.$data, this.$el);
  },
  created() {
    console.log("created", this.$data, this.$el);
  },
  beforeMount() {
    console.log("beforeMount", this.$data, this.$el);
  },
  mounted() {
    console.log("mounted", this.$data, this.$el);
  },
  beforeUpdate() {
    console.log("beforeUpdate", this.$data, this.$el);
  },
  updated() {
    console.log("updated", this.$data, this.$el);
  },
  beforeUnmount() {
    console.log("beforeUnmount", this.$data, this.$el);
  },
  unmounted() {
    console.log("unmounted", this.$data, this.$el);
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
