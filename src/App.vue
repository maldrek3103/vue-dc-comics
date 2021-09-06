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
ul {
  list-style-type: none;
}

ul li a {
  text-decoration: none;
  color: #000;
}
</style>
