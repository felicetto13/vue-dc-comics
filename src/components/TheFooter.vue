<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col py-5">
          <div class="row">
            <div class="col">
              <h4 class="text-uppercase fw-bold text-start">dc comics</h4>
              <ul class="list-unstyled">
                <li
                  class="p-1 text-menu"
                  v-for="link in comicsLinks"
                  :key="link"
                >
                  {{ link }}
                </li>
              </ul>
              <h4 class="text-uppercase fw-bold text-start">Shop</h4>
              <ul class="list-unstyled">
                <li class="p-1 text-menu" v-for="link in shopLinks" :key="link">
                  {{ link }}
                </li>
              </ul>
            </div>
            <div class="col">
              <h4 class="text-uppercase fw-bold text-start">dc</h4>
              <ul class="list-unstyled">
                <li class="p-1 text-menu" v-for="link in dcLinks" :key="link">
                  {{ link }}
                </li>
              </ul>
            </div>
            <div class="col">
              <h4 class="text-uppercase fw-bold text-start">sites</h4>
              <ul class="list-unstyled">
                <li
                  class="p-1 text-menu"
                  v-for="link in sitesLinks"
                  :key="link"
                >
                  {{ link }}
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col dc-logo-bg">
           
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      comicsLinks: [
        "Characters",
        "Comics",
        "movies",
        "tv",
        "games",
        "collectibles",
        "videos",
        "Fans",
        "news",
        "shop",
      ],
      shopLinks: ["Shop Dc", "shop dc collectibles"],
      dcLinks: [
        "Characters",
        "Comics",
        "movies",
        "tv",
        "games",
        "collectibles",
        "videos",
        "Fans",
        "news",
        "shop",
      ],
      sitesLinks: [
        "Characters",
        "Comics",
        "movies",
        "tv",
        "games",
        "collectibles",
      ],
    };
  },
};
</script>


<style lang="scss" scoped>
footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: top;
    background-repeat: no-repeat;
    background-size: cover;
}
h4 {
    color: white;
}
.text-menu {
  font-size: 0.8rem;
  color: darkgray;
  font-weight: 600;
}
.dc-logo-bg {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
</style>