<template>
  <div>
    <section class="form">
      <h1>
        New posts
      </h1>
      <AdminPostForm />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "~/components/Admin/AdminPostForm.vue";
export default {
  components: { AdminPostForm }
};
</script>

<style>
section.form {
  max-width: 90ch;
  margin: auto;
}
</style>
