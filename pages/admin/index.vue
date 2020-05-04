<template>
  <div class="admin-page">
    <aside>
      <button @click="$router.push('/admin/new-post')">Create post</button>
    </aside>
    <section class="existing-posts">
      <h1>Existing posts</h1>
      <PostList />
    </section>
  </div>
</template>
<script>
import PostList from "@/components/Posts/PostList";
export default {
  components: {
    PostList
  }
};
</script>
<style lang="scss" scoped></style>
