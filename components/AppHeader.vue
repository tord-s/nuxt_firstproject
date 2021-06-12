<template>
  <header class="header">
    <h1 class="title">Dad jokes</h1>
    <ul>
      <li>
        <nuxt-link to="/" exact class="btn">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/jokes" exact class="btn">Jokes</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/about" exact class="btn">About</nuxt-link>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "AppHeader"
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
  padding-bottom: 1rem;
}
.header ul {
  display: flex;
}
.header a {
  display: inline-block;
  padding: 0.3rem 1rem;
  margin-right: 0.5rem;
}
</style>
