<script setup>
import { ref, onMounted } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
const posts = ref([])

onMounted(async () => {
  const response = await fetch('/posts.json')
  posts.value = await response.json()
})
</script>

<template>
  <h1>{{ msg }}</h1>

  import { ref, onMounted } from 'vue'

  defineProps({
  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
    >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p>
    Learn more about IDE Support for Vue in the
    <a
        href="https://vuejs.org/guide/scaling-up/tooling.html#ide-support"
        target="_blank"
    >Vue Docs Scaling up Guide</a
    >.
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>

  <h2>Danh sách bài viết</h2>
  msg: String,
  })

  const count = ref(0)
  <ul>
    <li v-for="post in posts" :key="post.id">
      <h3>{{ post.title }}</h3>
      <p>{{ post.content }}</p>
    </li>
  </ul>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>