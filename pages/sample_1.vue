<template>
  <ul>
    <li><NuxtLink to="sample_1">sample_1</NuxtLink></li>
    <li><NuxtLink to="sample_2">sample_2</NuxtLink></li>
    <li><NuxtLink to="sample_3">sample_3</NuxtLink></li>
    <li><NuxtLink to="https://vue-draggable-next.vercel.app/#/">demo</NuxtLink></li>
  </ul>

  <h1>Favorite Foods</h1>
  <draggable v-model="meals" tag="ul">
    <template #item="{ element: meal }">
      <li>{{ meal }}</li>
    </template>
  </draggable>
</template>

<script setup lang="ts">
import draggable from "vuedraggable";
const meals = ref(["Hamburger", "Pizza", "Spaghetti", "Tacos", "Teriyaki Chicken"]);
</script>
