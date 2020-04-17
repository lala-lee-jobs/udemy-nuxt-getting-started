<template>
  <div>
    <h1>Users</h1>
    <div>
      <input type="text" v-model="userId" placeholder="Pleack input userId" />
      <button @click="onLoadUser">Load User</button>
    </div>
    <div>
      <nuxt-link to="/users/1">User 1 -> OK</nuxt-link>
    </div>
    <div>
      <nuxt-link to="/users/a">User a -> 404</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: '',
    };
  },
  methods: {
    onLoadUser() {
      this.$router.push(`/users/${this.userId}`);
    },
  },
};
</script>
