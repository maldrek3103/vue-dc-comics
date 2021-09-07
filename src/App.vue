<template>
  <div id="app">
    <Header />
    <main>
      <Content />
      <Links />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Content from "@/components/Content.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "App",

  components: {
    Header,
    Content,
    Footer,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
  list-style: none;
}
</style>
