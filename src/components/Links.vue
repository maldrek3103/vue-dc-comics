<template>
  <section id="more-links">
    <div class="container">
      <div>
        <h4>DC COMICS</h4>
        <ul>
          <li v-for="(link, index) in dcComics" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </div>
      <div>
        <h4>SHOP</h4>
        <ul>
          <li v-for="(link, index) in shop" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </div>
      <div>
        <h4>DC</h4>
        <ul>
          <li v-for="(link, index) in dc" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </div>
      <div>
        <h4>SITES</h4>
        <ul>
          <li v-for="(link, index) in sites" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </div>
    </div>
    <div class="container">
      <img src="../assets/img/dc-logo-bg.png" alt="" />
    </div>
  </section>
</template>

<script>
export default {
  name: "Links",
  data() {
    return {
      dcComics: [
        {
          text: "Characters",
          url: "#",
        },
        {
          text: "Comics",
          url: "#",
        },
        {
          text: "Movies",
          url: "#",
        },
        {
          text: "TV",
          url: "#",
        },
        {
          text: "Games",
          url: "#",
        },
        {
          text: "Videos",
          url: "#",
        },
        {
          text: "News",
          url: "#",
        },
      ],
      shop: [
        {
          text: "Shop DC",
          url: "#",
        },
        {
          text: "Shop DC Collectibles",
          url: "#",
        },
      ],
      dc: [
        {
          text: "Term Of Use",
          url: "#",
        },
        {
          text: "Privacy policy (New)",
          url: "#",
        },
        {
          text: "Ad Choices",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "Jobs",
          url: "#",
        },
        {
          text: "Subscriptions",
          url: "#",
        },
        {
          text: "Talent Workshops",
          url: "#",
        },
        {
          text: "CPSC Certificates",
          url: "#",
        },
        {
          text: "Ratings",
          url: "#",
        },
        {
          text: "Shop Help",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
      sites: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "MAD Magazine",
          url: "#",
        },
        {
          text: "DC Kids",
          url: "#",
        },
        {
          text: "DC Universe",
          url: "#",
        },
        {
          text: "DC Power Visa",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
#more-links {
  min-height: 370px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}
ul {
  display: flex;
  flex-direction: column;
}
li {
  list-style-type: none;
  margin: 0 1rem;
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