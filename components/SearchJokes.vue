<template>
  <form @submit.prevent="onSubmit" class="searchbar">
    <input
      class="query_input"
      type="text"
      v-model="text"
      placeholder="Seach Jokes..."
      v-on:input="updateResultLive"
    />
    <input
      v-if="text"
      class="btn query_btn"
      type="submit"
      value="Search Jokes"
    />
  </form>
</template>

<style scoped>
.searchbar {
  display: flex;
  justify-content: space-between;
  width: 100%;
}
.query_input {
  flex-grow: 7;
  border: none;
  font-size: 1.2rem;
  padding: 1rem;
}
.query_input:active,
.query_input:focus {
  outline: none;
}
.query_btn {
  flex-grow: 3;
  font-size: 1.2rem;
  max-height: 3rem;
  padding: 0;
  line-height: 0;
}
</style>

<script>
export default {
  name: "SeachJokes",
  data() {
    return {
      text: ""
    };
  },
  methods: {
    onSubmit() {
      this.$emit("search-text", this.text);
      this.text = "";
    },
    updateResultLive() {
      this.$emit("search-text", this.text);
    }
  }
};
</script>
