<template>
  <div>
    <h1>About something</h1>
    <p>A p tag content stuff</p>
  </div>
</template>

<script>
export default {
  transition: "default_fade",
  head() {
    return {
      title: "About The App",
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
