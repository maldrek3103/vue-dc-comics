<template>
  <div id="app" class="container">
    <Header />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
export default {
  name: "App",

  components: {
    Header,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
.container {
  max-width: 1200px;
  margin: auto;
}
ul {
  display: flex;
  list-style-type: none;
}
ul li {
  margin: 0 1rem;
}
ul li a {
  text-decoration: none;
  color: #000;
}
</style>
