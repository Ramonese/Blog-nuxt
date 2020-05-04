<template>
  <section class="posts-page layout">
    <h1>Posts</h1>
    <div class="post-container">
      <PostFeatured
        id="1"
        title="Title 1"
        text="Apparently we had reached a great
      height in the atmosphere, for the sky was a dead black, and the stars had
      ceased to twinkle. By the same illusion which lifts the horizon of the sea
      to the level of the spectator on a hillside."
      />
    </div>
  </section>
</template>

<script>
import PostFeatured from "@/components/Posts/PostFeatured";
export default {
  components: {
    PostFeatured
  }
};
</script>

<style scoped>
.posts-page {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
