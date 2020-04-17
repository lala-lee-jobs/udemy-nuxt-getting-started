<template>
  <div>
    Users
    <input type="text" v-model="userId" placeholder="Pleack input userId" />
    <button @click="onLoadUser">Load User</button>
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
