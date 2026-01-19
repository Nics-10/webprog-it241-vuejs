<template>
  <div class="banana">
    <h2>{{ name }}</h2>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  name: 'FoodItem2',
  data() {
    return {
      name: 'Bananas are yellow',
      message: 'My favorite color is yellow so I like banana'
    }
  }
}
</script>

<style>
.banana {
  border: dashed black 1px;
  display: inline-block;
  margin: 10px;
  padding: 10px;
  background-color: rgb(255, 243, 6);
}
</style>