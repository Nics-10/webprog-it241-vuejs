<template>
  <div>
    <PersonalProfile />

    <div class="fruits-section">
      <h1>Fruits</h1>
      <food-item />
      <food-item2 />
    </div>
  </div>
</template>

<script>
import PersonalProfile from './components/PersonalProfile.vue'
import FoodItem from './components/FoodItem.vue'
import FoodItem2 from './components/FoodItem2.vue'

export default {
  name: 'App',
  components: {
    PersonalProfile,
    FoodItem,
    FoodItem2
  }
}
</script>

<style>
.fruits-section {
  margin-top: 50px;
  text-align: center;
}
</style>