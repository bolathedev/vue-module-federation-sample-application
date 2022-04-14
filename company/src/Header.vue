<template>
  <div>
    <header>
      <h2>App Header which is served from company app</h2>
      <p>items: {{ cartCount }}</p>
    </header>
  </div>
</template>

<script>
export default {
  computed: {
    cartCount() {
      return this.$store.state.cartItems;
    },
  },
};
</script>
