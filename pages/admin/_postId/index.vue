// pages/_postId/index.vue
<template>
  <div class="admin-post-page">
    <section class="update-form">
      <!-- Add a post update form component -->
      <AdminPostForm v-bind:post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm";

export default {
  components: {
    AdminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: "Gaylon",
        title: "My awesome Post",
        content: "Super amazing content, thanks for that!",
        thumbnailLink:
          "https://vignette.wikia.nocookie.net/ncaa-athletics/images/7/73/Georgia_Tech_Yellow_Jackets.jpg/revision/latest?cb=20180311011603"
      }
    };
  }
};
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>
