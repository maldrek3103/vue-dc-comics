<template>
  <div id="app">
    <Header />
    <main>
      <Content />
      <Services />
      <Links />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Content from "@/components/Content.vue";
import Services from "@/components/Services.vue";
import Links from "@/components/Links.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "App",

  components: {
    Header,
    Content,
    Services,
    Links,
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
