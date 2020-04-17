<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="onLoadUser">Load User</button>
  </div>
</template>
<script>
export default {
  layout: 'header-main',
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