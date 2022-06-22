<template>
  <div class="container">
    <nav class="my-navbar">
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
.my-navbar {
    display: flex;
    justify-content: space-between;
    padding: 0.1rem 0;

    ul {

        margin: 0;

        li {
            position: relative;
            padding-top: 1.5rem;
            &:after {
                transform: scaleY(0);
                position: absolute;
                width: 100%;
                bottom: 0;
                content: '';
                height: 5px;
                background-color: #0082f9;
                transition:.3s;
                transition-property: transform;
                transform-origin: bottom;
                transition-timing-function: ease-in-out;
            }
            &:hover:after{
                transform: scaleY(1);
            }
        }
        
    }  
}

.nav-link {
    padding: 1rem 1rem;
    font-weight: bold;
    color:dimgray;
}
</style>