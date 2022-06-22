<template>
  <div>
    <div class="card-image">
      <img :src="img" :alt="serie" />
    </div>

    <div class="card-body">
      <div class="card-title text-uppercase">{{ serie }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    img: String,
    price: String,
    serie: String,
    type: String,
  },
};
</script>

<style lang="scss" scoped>
.card-image {
  height: 200px;
  overflow: hidden;
  width: 100%;

    img {
        width: 100%;
    }
}

.card-body{
    .card-title {
        font-size: .9rem;
        padding: .5rem 0;
        color: white;
    }
}
</style>