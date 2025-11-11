<template>
  <section id="contact">
    <div class="container">
      <div class="contact">
        <h2>Let's Not Connect</h2>
        <p>Hesitate to reach out! I am not open to anything.</p>
        <div class="contact-links">
          <a :href="`mailto:${email}`" class="contact-btn">
            📧 I'll never give you my email
          </a>
          <a :href="github" class="contact-btn secondary" target="_blank" rel="noopener noreferrer">
            🐙 GitHub
          </a>
          <a :href="linkedin" class="contact-btn secondary" target="_blank" rel="noopener noreferrer">
            💼 LinkedIn
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import '../assets/contact.css'

export default {
  name: 'ContactSection',
  data() {
    return {
      email: 's1146063@mail.yzu.edu.tw',
      github: 'https://github.com/bycrn',
      linkedin: 'https://www.linkedin.com/in/rahmanicerine/'
    }
  }
}
</script>
