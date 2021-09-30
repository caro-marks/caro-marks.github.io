<template>
  <div class="testin">
    <div class="container">
      <section>
        <h5 class="title">Lista teste</h5>
        <ul>
          <li v-for="(value, key) in stuffs" :key="key">
            <p>{{ key }}</p>
          </li>
        </ul>
      </section>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import axios from '@/utils/axios'

export default defineComponent({
  data() {
    return {
      stuffs: []
    }
  },
  created() {
    this.fetchingData()
  },
  methods: {
    async fetchingData() {
      const { data } = await axios.get('/sample.json')
      this.stuffs = data
    }
  }
})
</script>

<style></style>
