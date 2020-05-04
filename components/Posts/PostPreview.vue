<template>
  <nuxt-link :to="postLink">
    <article>
      <h3>{{ title }}</h3>
      <h4>{{ author }}</h4>
      <p>{{ text }}</p>
    </article>
  </nuxt-link>
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
    },
    author: {
      type: String,
      default: "author"
    },
    isAdmin: {
      type: Boolean,
      required: true
    }
  },
  computed: {
    postLink() {
      return this.isAdmin ? "/admin/" + this.id : "/posts/" + this.id;
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
