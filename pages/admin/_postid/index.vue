<template>
  <div class="admin-post-page">
    <section>
      <h1>Edit</h1>
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "~/components/Admin/AdminPostForm.vue";
export default {
  components: { AdminPostForm },
  data() {
    return {
      loadedPost: {
        author: "Ieva",
        title: "Fancy post",
        image: "",
        content: "content"
      }
    };
  }
};
</script>
