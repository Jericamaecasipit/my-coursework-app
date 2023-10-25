<template>
    <div class="bg-white p-4 rounded shadow-lg mb-4">
      <h2 class="text-xl font-semibold">{{ coursework.title }}</h2>
      <p class="text-gray-600">{{ coursework.description }}</p>
      <p class="text-gray-500">{{ coursework.dueDate }}</p>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      coursework: Object,
    },
  };
  </script>
  