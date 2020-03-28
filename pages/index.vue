<template>
  <div class="container">
    <section>
      <h1>Latest posts</h1>
    </section>
    <section class="featured-posts">
      <article>
        <h2>Title 1</h2>
        <p>excerpt</p>
        <nuxt-link :to="'/posts/' + 1">read more</nuxt-link>
      </article>
      <article>
        <h2>Title 2</h2>
        <p>
          Apparently we had reached a great height in the atmosphere, for the
          sky was a dead black, and the stars had ceased to twinkle. By the same
          illusion which lifts the horizon of the sea to the level of the
          spectator on a hillside
        </p>
        <nuxt-link :to="'/posts/' + 2">read more</nuxt-link>
      </article>
      <article>
        <h2>Title 1</h2>
        <p>excerpt</p>
        <nuxt-link :to="'/posts/' + 1">read more</nuxt-link>
      </article>
      <article>
        <h2>Title 2</h2>
        <p>
          Apparently we had reached a great height in the atmosphere, for the
          sky was a dead black, and the stars had ceased to twinkle. By the same
          illusion which lifts the horizon of the sea to the level of the
          spectator on a hillside
        </p>
        <nuxt-link :to="'/posts/' + 2">read more</nuxt-link>
      </article>
    </section>
  </div>
</template>

<script>
export default {
  components: {}
};
</script>

<style>
.container {
  margin: 0 auto;
  padding: 1em;
}

.title {
  color: #35495e;
  letter-spacing: 1px;
}
.featured-posts {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  grid-template-rows: 200px 200px;
  grid-gap: 20px 30px;
}
.featured-posts article {
  background: cornflowerblue;
}
</style>
