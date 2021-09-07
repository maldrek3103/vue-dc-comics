<template>
  <section id="services">
    <div>
      <ul>
        <li v-for="(service, index) in services" :key="index">
          <a :href="service.url"
            ><img :src="service.img" />{{ service.text }}</a
          >
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "Services",
  data() {
    return {
      services: [
        {
          text: "DIGITAL COMICS",
          url: "#",
          img: "../assets/img/buy-comics-digital-comics.png",
        },
        {
          text: "DC MERCHANDISE",
          url: "#",
          img: "../assets/img/buy-comics-merchandise.png",
        },
        {
          text: "SUBSCRIPTION",
          url: "#",
          img: "../assets/img/buy-comics-subscription.png",
        },
        {
          text: "COMIC SHOP LOCATION",
          url: "#",
          img: "../assets/img/buy-comics-shop-locator.png",
        },
        {
          text: "DC POWER VISA",
          url: "#",
          img: "../assets/img/buy-comics-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
#services {
  min-height: 155px;
  background-color: aqua;
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
}

a {
  text-decoration: none;
  text-transform: uppercase;
  color: #000;
}
</style>