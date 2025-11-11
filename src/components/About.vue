<template>
  <section id="about" class="about">
    <div class="container">
      <div class="about-content">
        <img :src="profilePhoto" alt="Your Name" class="profile-photo">
        <div>
          <h1>Cerine RAHMANI</h1>
          <p class="tagline">Student | Developer | Business Analyst IT</p>
          <p class="bio">
            I'm a french student currently studying in Taiwan in the computer science & engineering department, pursuing coursework in computer science, data science, research in digital game and management. 
            I'm passionate about programming and 3D graphics.
            When I'm not coding, you can find me drawing or planning my next travel to escape and eat halal food.
          </p>
          <div class="skills">
            <span v-for="skill in skills" :key="skill" class="skill-tag">{{ skill }}</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import '../assets/about.css'

export default {
  name: 'AboutSection',
  data() {
    return {
      profilePhoto: '/src/assets/profile.jpg',
      skills: [
        'C++',
        'Python',
        'PL/SQL',
        'JavaScript',
        'Vue.js',
        'Three.js'      
      ]
    }
  }
}
</script>

