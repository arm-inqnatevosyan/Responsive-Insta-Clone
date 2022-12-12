<template>
  <div>
    <Navbar />
    <Story />
    <Posts />
  </div>
</template>
<script>
import Navbar from '~/components/Navbar.vue'
import Story from '~/components/story/Story.vue'
import Posts from '~/components/posts/Posts.vue'

export default {
  components: { Navbar, Story, Posts }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
