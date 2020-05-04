<template>
  <article>
    <h3>{{ title }}</h3>
    <p>{{ text }}</p>
  </article>
</template>

<script>
export default {
  name: "PostPreview",
  props: {
    id: {
      type: String,
      required: true
    },
    title: {
      type: String,
      default: "Title of post preview"
    },
    text: {
      type: String,
      default: "Apparently we had reached a great height"
    }
  }
};
</script>

<style scoped>
article {
  padding: 1em;
}
h3 {
  font-size: 3rem;
}
</style>
