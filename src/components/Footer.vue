<template>
  <footer>
    <p> Just some text</p>
    <router-link v-show="homePage" to="/about">About</router-link>
  </footer>
</template>

<script>
export default {
  computed: {
    homePage() {
      return this.$route.path === '/';
    }
  }
}
</script>

<style scoped>
a {
  color: #333
}

footer {
  margin-top: 30px;
  text-align: center;
}
</style>