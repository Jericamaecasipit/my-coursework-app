<template>
    <div>
      <h1 class="text-2xl font-semibold mb-4 ">Coursework List</h1>
      <CourseworkItem v-for="item in courseworkList" :key="item.id" :coursework="item" />
    </div>
  </template>
  <script>
  import CourseworkItem from './CourseworkItem.vue';
  export default {
    components: {
      CourseworkItem, 
    },
    data() {
       return { 
        courseworkList: [
          {
            id: 1,
            title: 'Homework 1',
            description: 'Complete exercises 1-5.',
            dueDate: '2023-10-15',
          },
          {
            id: 2,
            title: 'Project Proposal',
            description: 'Submit your project proposal.',
            dueDate: '2023-10-20',
          },
        ],
      };
    },
  };
  </script>
  