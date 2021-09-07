<template>
  <header>
    <div>
      <img src="../assets/img/dc-logo.png" alt="Logo" />
    </div>
    <div>
      <ul id="navbar">
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
header {
  min-height: 120px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

div {
  max-width: 1200px;
  margin: 0 auto;
}

ul {
  display: flex;
}

li {
  list-style-type: none;
  margin: 0 1rem;
  line-height: 115px;
}

a {
  text-decoration: none;
  text-transform: uppercase;
  color: #000;
}

li:hover {
  border-bottom: 5px solid blue;
  color: blue;
}
</style>
