<template>
  <div class="home">
    <header>
      <h1>{{ allData.general.title }}</h1>
      <section>
        <h2 v-for="name in allData.general.names" :key="name.id">
          {{ name }}
        </h2>
        <img src="@/static/images/selfie.jpeg" alt="" />
      </section>
      <div class="container">
        <h2>General info</h2>
        <ul>
          <li v-for="(value, key) in allData.general.presentation" :key="key">
            <p>{{ value }}</p>
          </li>
        </ul>
      </div>
    </header>
    <body>
      <h2>Skills</h2>
      <div class="skills">
        <section class="container">
          <h3>Advanced</h3>
          <ul>
            <li v-for="(value, key) in allData.skills.advanced" :key="key">
              <p>{{ value }}</p>
            </li>
          </ul>
        </section>
        <section class="container">
          <h3>Advancing</h3>
          <ul>
            <li v-for="(value, key) in allData.skills.medium" :key="key">
              <p>{{ value }}</p>
            </li>
          </ul>
        </section>
        <section class="container">
          <h3>Soft</h3>
          <ul>
            <li v-for="(value, key) in allData.skills.complementars" :key="key">
              <p>{{ value }}</p>
            </li>
          </ul>
        </section>
      </div>
      <h2>Experiences</h2>
      <div class="experiences">
        <section class="container">
          <h3>Professional</h3>
          <ul>
            <li
              v-for="(value, key) in allData.experiences.professional"
              :key="key"
            >
              <p>{{ value }}</p>
            </li>
          </ul>
        </section>
        <section class="container">
          <h3>Educational</h3>
          <ul>
            <li v-for="(value, key) in allData.experiences.scholars" :key="key">
              <p>{{ value }}</p>
            </li>
          </ul>
        </section>
      </div>
    </body>
    <footer>
      <div class="container">
        <h2>Hire me!</h2>
        <h3>Contacts</h3>
        <div>
          <p>{{ allData.contacts.email }}</p>
          <p>{{ allData.contacts.phone }}</p>
        </div>
        <a href="{{allData.contacts.linkedin}}">Linkedin</a>
        <a href="{{allData.contacts.github}}">Github</a>
      </div>
    </footer>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import axios from '@/utils/axios'

export default defineComponent({
  data() {
    return {
      allData: []
    }
  },
  methods: {
    async fetchData() {
      const { data } = await axios.get('/info.json')
      this.allData = data
    }
  },
  created() {
    this.fetchData()
  }
})
</script>

<style scoped>
.skills {
  columns: 20vh 3;
}

.experiences {
  columns: 30vh 2;
  /* column-rule: 20vh double; */
}

.container {
  margin: 4rem auto;
  max-width: 500px;
  width: 90%;
  display: grid;
  grid-gap: 2.5rem;
}

.title {
  font-size: 1rem;
  font-weight: 500;
  margin: 0.7rem 0;
}

header {
  padding: 2rem 0 4rem;
  text-align: center;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

header img {
  max-width: 150px;
  border-radius: 50px;
}

p {
  margin: 0;
}

ul {
  padding: 0;
  margin: 0;
  display: grid;
  grid-gap: 1rem;
}

li {
  background-color: #2b3a4e;
  padding: 1.2rem 1rem;
  border-radius: 1rem;
  position: relative;
  list-style: none;
  color: #8b98a8;
}
</style>
