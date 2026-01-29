<template>
  <div class="comment-box">
    <h1>Comments</h1>
    <ul class="comment-list">
      <li v-for="comment in comments" :key="comment.id" class="comment-item">
        <strong>{{ comment.name }}:</strong>
        <p>{{ comment.comment }}</p>
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
  margin-top: 2rem;
  padding: 1rem;
  background-color: #fffbe6;
  border: 1px dashed #999;
  border-radius: 8px;
}

.comment-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.comment-item {
  background-color: #fefefe;
  border: 1px solid #ddd;
  border-radius: 6px;
  padding: 0.75rem;
  margin-bottom: 1rem;
  box-shadow: 0 1px 3px rgba(0,0,0,0.1);
}

.comment-item strong {
  color: #333;
  font-size: 1rem;
}

.comment-item p {
  margin: 0.5rem 0 0;
  color: #555;
}
</style>