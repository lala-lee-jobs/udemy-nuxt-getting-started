<template>
  <div class="container">
    <nuxt-link to="/users">Users</nuxt-link>
    <!-- <nuxt-link to="/products">Products</nuxt-link> -->
    <button @click="onLoadProducts">Load Products</button>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo,
  },
  methods: {
    onLoadProducts() {
      this.$router.push('/products');
    },
  },
}
</script>

