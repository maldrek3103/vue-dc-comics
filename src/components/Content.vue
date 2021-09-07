<template>
  <section id="main-content">
    <div><h3>Content goes here</h3></div>
  </section>
</template>

<script>
export default {
  name: "Content",
};
</script>

<style scoped lang="scss">
#main-content {
  height: 140px;
  background-color: black;
}
section {
  display: flex;
  align-items: center;
}
div {
  max-width: 1200px;
  margin: 0 auto;
}
h3 {
  font-weight: bold;
  color: #fff;
}
</style>