<template>
  <article>
    <h2>{{ title }}</h2>
    <p>{{ text }}</p>
    <nuxt-link :to="'/posts/' + id">read more</nuxt-link>
  </article>
</template>

<script>
export default {
  name: "PostFeatured",
  props: {
    id: {
      type: String,
      required: true
    },
    title: {
      type: String,
      default: "Title"
    },
    text: {
      type: String,
      required: "Apparently we had reached a great height"
    }
  }
};
</script>

<style scoped>
article {
  background: cornflowerblue;
  padding: 1em;
}
h2 {
  font-size: 3rem;
}
</style>
