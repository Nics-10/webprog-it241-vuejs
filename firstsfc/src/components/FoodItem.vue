<template>
  <div>
    <h2>{{ name }}</h2>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'Apples are red',
      message: 'My favorite color is red so I like apples'
    }
  }
};
</script>

<style></style>