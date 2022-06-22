<template>
  <div id="app">
    <TheHeader></TheHeader>
    <main>
      <MainContent></MainContent>
    </main>
    <div class="banner bg-blue">
      <BannerBlue></BannerBlue>
    </div>
    <TheFooter></TheFooter>
    <div class="sign-up-banner">
      <div class="container">
        <div class="row">
          <div class="col justify-content-start">
            <button class="btn my-btn-primary">SIGN-UP NOW!</button>
          </div>
          <div class="col d-flex gap-5 justify-content-end align-self-center">
            <h2 class="text-blue">FOLLOW US</h2>
            <ul class="list-unstyled d-flex">
              <li v-for="(social,i) in socialItems" :key="i" class="social-icon">
              <img :src="require('/src/assets/img/footer-'+ social.img)" :alt="social.name"></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import BannerBlue from "./components/BannerBlue.vue";
import MainContent from "./components/MainContent.vue";
export default {
  name: "App",
  components: {
    TheHeader,
    TheFooter,
    BannerBlue,
    MainContent
  },
  data() {
    return {
      socialItems:
      [
        {
          name: "facebook",
          img: "facebook.png",
        },
        {
          name: "twitter",
          img: "twitter.png",
        },
        {
          name: "youtube",
          img: "youtube.png",
        },
        {
          name: "pinterest",
          img: "pinterest.png",
        },
        {
          name: "periscope",
          img: "periscope.png",
        }
      ]
    }
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.main-content {
  background-color: black;
  color: white;
  font-size: 30px;
  text-align: center;
  padding: 5rem 0;
}
.banner {
  padding: 5rem 0;
}
.bg-blue {
  background-color: #0082f9;
  color: white;
}

.sign-up-banner {
  background-color: #303030;
  padding: 2rem 0;
}
.sign-up-banner .my-btn-primary {
  background-color: transparent;
  color: white;
  border-color: #0082f9;
  border-radius: 0;
  border-width: 2px;
  padding: 1rem 1.5rem;
}
.text-blue {
  color: #0082f9;
}
.social-icon {
  padding: 0 .5rem;
}
</style>
