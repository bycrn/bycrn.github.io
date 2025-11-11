<template>
  <div id="app">
    <NavigationBar />
    <AboutSection />
    <ProjectsSection />
    <ContactSection />
    <footer>
      <div class="container">
        <p>&copy; 2025 bycrn. Built with Vue.js and deployed on GitHub Pages.</p>
      </div>
    </footer>
  </div>
</template>

<script>
import NavigationBar from './components/NavigationBar.vue'
import AboutSection from './components/About.vue'
import ProjectsSection from './components/Projects.vue'
import ContactSection from './components/Contact.vue'
// Import des styles globaux
import './assets/variables.css'
import './assets/global.css'

export default {
  name: 'App',
  components: {
    NavigationBar,
    AboutSection,
    ProjectsSection,
    ContactSection
  }
}
</script>
