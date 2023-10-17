<template>
  <div class="product">
    <div class="product__name">Name: {{ name }}</div>
    <div class="product__price">Price: {{ formattedPrice }}</div>
    <div v-if="available" class="product__available">Available</div>
    <div v-else class="product__available">Out of stock</div>
  </div>
</template>

<script>
export default {
  name: "ProductDetails",
  data() {
    return {
      name: 'Smartphone',
      price: 99.99,
      available: true,
    }
  },
  computed: {
    formattedPrice() {
      return `$${this.price}`;
    }
  }
}
</script>

<style scoped>
.product {
  border: 1px solid gray;
  border-radius: 16px;
  padding: 16px 32px;
  align-self: center;
}
</style>