<template>
  <section id="services">
    <ul>
      <li><a href="#">digital comics</a></li>
      <li><a href="#">dc merch</a></li>
      <li><a href="#">sub</a></li>
      <li><a href="#">shop</a></li>
      <li><a href="#">dc visa card</a></li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "Services",
};
</script>

<style scoped lang="scss">
#services {
  height: 160px;
  background-color: #123;
}
#services ul {
  display: flex;
  justify-content: space-between;
}
#services ul li a {
  color: #fff;
}
</style>