<template>
  <div class="container">
    <section class="featured-posts">
      <PostFeatured
        title="Title 1"
        text="Apparently we had reached a great
      height in the atmosphere, for the sky was a dead black, and the stars had
      ceased to twinkle. By the same illusion which lifts the horizon of the sea
      to the level of the spectator on a hillside."
        id="1"
      />
      <PostFeatured
        title="Title 2"
        text="Apparently we had reached a great
      height in the atmosphere, for the sky was a dead black."
        id="2"
      />
      <PostFeatured
        title="Title 3"
        text="Apparently we had reached a great
      height in the atmosphere, for the sky was a dead black, and the stars had
      ceased to twinkle. By the same illusion which lifts the horizon of the sea
      to the level of the spectator on a hillside."
        id="3"
      />
      <PostFeatured
        title="Title 3"
        text="Apparently we had reached a great
      height in the atmosphere, for the sky was a dead black, and the stars had
      ceased to twinkle. By the same illusion which lifts the horizon of the sea
      to the level of the spectator on a hillside."
        id="3"
      />
    </section>
  </div>
</template>

<script>
import PostFeatured from "~/components/Posts/PostFeatured";
export default {
  components: {
    PostFeatured
  }
};
</script>

<style>
.container {
  margin: 0 auto;
  padding: 1em;
}

.featured-posts {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  grid-template-rows: auto auto;
  grid-gap: 20px 30px;
}
</style>
