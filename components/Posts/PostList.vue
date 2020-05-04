<template>
  <div class="post-list">
    <PostPreview
      id="4"
      author="andris"
      :is-admin="isAdmin"
      text="some text"
      title="First title"
    />
    <PostPreview
      id="5"
      author="ieva"
      title="Some other title"
      :is-admin="isAdmin"
      text="some other text"
    />
  </div>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";
export default {
  name: "PostList",
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
};
</script>
<style>
a {
  text-decoration: underline;
}
</style>
