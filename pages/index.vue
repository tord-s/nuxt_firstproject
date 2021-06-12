<template>
  <div>
    <h2>Welcome to a dad jokes app</h2>
  </div>
</template>

<script>
export default {
  transition: "default_fade",
  head() {
    return {
      title: "Welcome To The App",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Best place for corny dad jokes"
        }
      ]
    };
  }
};
</script>
