<template>
  <header>
    <ul>
      <li>Home</li>
      <li>Services</li>
      <li>About</li>
      <li>Resume</li>
      <li>Blog</li>
      <li>Contact</li>
    </ul>
  </header>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  data() {
    return {
      testin: []
    }
  },
  created() {
    this.fetchingData()
  },
  methods: {
    async fetchingData() {
      const { data } = await axios.get('/users')
      this.testin = data
    }
  }
})
</script>
