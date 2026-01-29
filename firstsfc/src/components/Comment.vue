<template>
  <div class="comment-box">
    <h1>Comments</h1>
    <ul>
      <li v-for="comment in comments" :key="comment.id">
        <strong>{{ comment.name }}:</strong> {{ comment.comment }}
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import { supabase } from '../lib/supabaseClient'

const comments = ref([])

async function getComments() {
  const { data, error } = await supabase.from('comments').select()
  if (error) {
    console.error('Error fetching comments:', error)
  } else {
    comments.value = data
  }
}

onMounted(() => {
  getComments()
})
</script>

<style scoped>
.comment-box {
  border: dashed black 1px;
  display: block;
  margin: 10px;
  padding: 10px;
  background-color: lightyellow;
}
</style>