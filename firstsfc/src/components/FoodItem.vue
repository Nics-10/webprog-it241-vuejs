<template>
  <div class="apple">
    <h2>{{ name }}</h2>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  name: 'FoodItem',
  data() {
    return {
      name: 'Apples are red',
      message: 'My favorite color is red so I like apples'
    }
  }
}
</script>

<style scoped>
.apple {
  border: dashed black 1px;
  display: inline-block;
  margin: 10px;
  padding: 10px;
  background-color: red;
  color: white;
}
</style>