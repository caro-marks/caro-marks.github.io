<template>
  <div class="home">
    <section class="header">
      <div class="hello">
        <h1>{{ title }}</h1>
        <div>
          <h2>I'm {{ names[0] }} {{ names[3] }}!</h2>
          <ul class="world container">
            <li v-for="value in general" :key="value.id">
              <p>{{ value }}</p>
            </li>
          </ul>
        </div>
      </div>
      <img src="@/static/images/selfie.jpeg" alt="Me smiling at a pic" />
    </section>
    <section class="body">
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
          <h3>Improving</h3>
          <ul>
            <li v-for="(value, key) in allData.skills.medium" :key="key">
              <p>{{ value }}</p>
            </li>
          </ul>
        </section>
        <section class="container">
          <h3>Complementary</h3>
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
    </section>
    <section class="footer">
      <h2>Contact me!</h2>
      <div class="contacts">
        <a href=""><strong>E-mail</strong> : marcosabn08@gmail.com</a>
        <a href=""><strong>WhatsApp</strong> : +55 53 99701 0399</a>
        <a href="https://www.linkedin.com/in/caro-marks"
          ><strong>Linkedin</strong>: /in/caro-marks</a
        >
        <a href="https://www.github.com/caro-marks"
          ><strong>Github</strong>: /caro-marks</a
        >
      </div>
    </section>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import axios from '@/utils/axios'

export default defineComponent({
  data() {
    return {
      allData: [],
      title: '',
      names: [],
      general: []
    }
  },
  methods: {
    async fetchData() {
      const { data } = await axios.get('/info.json')
      this.allData = data
      this.title = data.general.title
      this.names = data.general.names
      this.general = data.general.presentation
    }
  },
  created() {
    this.fetchData()
  }
})
</script>

<style scoped>
.home {
  display: grid;
  grid-auto-flow: row;
  row-gap: 0.5rem;
}

.header {
  padding: 2rem 0 4rem;
  text-align: center;
  display: grid;
  grid-auto-flow: column;
}

.header img {
  width: 80%;
  max-width: 300px;
  border-radius: 50px;
  margin: auto;
}

.hello {
  display: grid;
  grid-auto-flow: row;
  row-gap: 2.5em;
}

.world {
  grid-gap: 1.5rem;
}

.body {
  text-align: center;
  display: grid;
  grid-auto-flow: row;
}

.skills {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  column-gap: 2.5%;
}

.experiences {
  display: grid;
  grid-template-columns: 1fr 1fr;
  column-gap: 5%;
}

.container {
  margin: 4rem auto;
  max-width: 500px;
  width: 90%;
  display: grid;
}

.footer {
  display: grid;
  grid-template-columns: 1fr 1fr;
  text-align: center;
}

.contacts {
  display: grid;
  grid-auto-flow: row;
  row-gap: 0.5rem;
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

a {
  text-decoration: none;
  color: whitesmoke;
}
</style>
