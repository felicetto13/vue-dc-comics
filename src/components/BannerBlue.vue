<template>
  <div class="container">
    <div class="row">
      <div class="col" v-for="(card, i) in cardLinks" :key="i">
        <div class="my-card">
          <div class="card-image">
            <img
              :src="require('../assets/img/buy-' + card.image)"
              :alt="card.title"
            />
          </div>
          <div class="card-title">
            <h3>{{ card.title }}</h3>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cardLinks: [
        {
          title: "digital comics",
          image: "comics-digital-comics.png",
        },
        {
          title: "dc merchandise",
          image: "comics-merchandise.png",
        },
        {
          title: "subscription",
          image: "comics-subscriptions.png",
        },
        {
          title: "digital comics",
          image: "comics-shop-locator.png",
        },
        {
          title: "dc power visa",
          image: "dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>
<style lang="scss">
.my-card {
  display: flex;
  align-items: center;
  gap: 1rem;

      img{
            width: 70px;
            object-fit: contain;
            aspect-ratio: 1;
        }
      .card-title h3{
      font-size: .9rem;
      text-transform: uppercase;
        }
}
</style>

