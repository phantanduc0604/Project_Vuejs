<script>
export default {
  data() {
    return {
      name: "Danny",
      status: true,
      tasks: [
        'Task One', 'Task Two', 'Task Three'
      ],
      link: 'https://google.com '
    }
  },
  methods: {
    toggleStatus() {
      
    }
  }
}
</script>

<template>
   <h1>{{ name }}</h1>
   <p v-if="status">Active</p>
   <h3>Tasks:</h3>
   <ul>
    <li v-for="task in tasks" :key="task">{{ task }}</li>
   </ul>
   <a :href="link">Click to google</a>
   <button @click="toggleStatus">Change status</button>
</template>


