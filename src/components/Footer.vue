<template>
  <footer id="footer">
    <!-- Services -->
    <section id="services">
      <div class="container">
        <ul>
          <li v-for="(service, index) in services" :key="index">
            <a :href="service.url"
              ><img :src="service.img" />{{ service.text }}</a
            >
          </li>
        </ul>
      </div>
    </section>

    <!-- More Links -->
    <section id="more-links">
      <div class="container">
        <div class="links">
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
        <div class="links-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </section>

    <!-- Socials -->
    <section id="socials">
      <div class="container">
        <div>
          <button>Sign-up Now</button>
        </div>
        <div>
          <h5><a href="#">Follow Us</a></h5>
          <ul>
            <li v-for="(links, index) in socials" :key="index"></li>
          </ul>
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: "Footer",
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
      socials: [
        {
          text: "Facebook",
        },
        {
          text: "Twitter",
        },
        {
          text: "YouTube",
        },
        {
          text: "Pinterest",
        },
        {
          text: "Geo",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.container {
  max-width: 1200px;
  margin: 0 auto;
}
#services {
  background-color: #0282f9;
}
#services ul {
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding: 50px;
}
#services a {
  text-decoration: none;
  color: #fff;
}

#more-links {
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
#more-links .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
#more-links h4 {
  color: #fff;
}
#more-links a {
  text-decoration: none;
  color: #959595;
}

#socials {
  background-color: #303030;
}
#socials .container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
#socials .container div {
  padding: 2rem 0;
}
</style>