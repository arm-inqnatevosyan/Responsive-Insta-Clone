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
