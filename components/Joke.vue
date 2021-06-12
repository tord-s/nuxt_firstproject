<template>
  <nuxt-link :to="'jokes/' + id">
    <div class="joke btn">
      <p>{{ joke }}</p>
    </div>
  </nuxt-link>
</template>

<script>
export default {
  name: "Joke",
  props: ["joke", "id"]
};
</script>

<style scoped>
.joke {
  padding: 1rem;
  margin: 0.5rem 0;
}
</style>
