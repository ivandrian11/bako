<template>
  <div class="card shadow card-product">
    <img :src="'assets/img/' + product.gambar" class="card-img-top" />
    <div class="card-body">
      <h5 class="card-title">{{ product.nama }}</h5>
      <p class="card-text">Harga: Rp{{ product.harga }}</p>
      <router-link :to="'/product/' + product.id" class="btn btn-success">
        <b-icon-cart></b-icon-cart> Pesan
      </router-link>
    </div>
  </div>

  <!-- ../assets/img/hero.png -->
</template>

<script>
export default {
  name: "CardProduct",
  props: ["product"],
};
</script>

<style>
</style>