// components/Posts/PostList.vue
<template>
  <section class="post-list">
    <PostPreview
      id="1"
      thumbnail="https://vignette.wikia.nocookie.net/ncaa-athletics/images/7/73/Georgia_Tech_Yellow_Jackets.jpg/revision/latest?cb=20180311011603"
      title="Hello there!"
      previewText="This is my first post!"
    />
    <PostPreview
      id="2"
      thumbnail="https://vignette.wikia.nocookie.net/ncaa-athletics/images/7/73/Georgia_Tech_Yellow_Jackets.jpg/revision/latest?cb=20180311011603"
      title="Hello again!"
      previewText="This is my second post!"
    />
    <PostPreview
      id="3"
      thumbnail="https://vignette.wikia.nocookie.net/ncaa-athletics/images/7/73/Georgia_Tech_Yellow_Jackets.jpg/revision/latest?cb=20180311011603"
      title="Hello the third time!"
      previewText="This is my third post!"
    />
  </section>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";

export default {
  components: {
    PostPreview
  }
};
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>