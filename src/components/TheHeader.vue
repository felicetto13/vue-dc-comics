<template>
  <div class="container py-2">
    <nav class="navbar">
      <img src="../assets/img/dc-logo.png" alt="" />
      <ul class="d-flex list-unstyled">
        <li class="nav-item" v-for="(link, i) in navbarLink" :key="i">
          <a class="nav-link text-uppercase" href="#">{{ link }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navbarLink: [
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
    };
  },
};
</script>


<style lang="scss" scoped>


.nav-link {
    padding: 1rem 1rem;
    font-weight: bold;
    color:dimgray;
}
</style>