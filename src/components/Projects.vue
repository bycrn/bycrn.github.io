<template>
  <section id="projects" class="projects-section">
    <div class="container">
      <h2 class="section-title">Featured Projects</h2>
      <div class="projects-grid">
        <div v-for="project in projects" :key="project.title" class="project-card">
          <div class="project-icon">{{ project.icon }}</div>
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
          <a :href="project.githublink" class="project-link" target="_blank" rel="noopener noreferrer">It may be on my GitHub (if it's not in private)</a>
          <div class="project-tech">
            <span v-for="tech in project.technologies" :key="tech" class="tech-badge">
              {{ tech }}
            </span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import '../assets/projects.css'

export default {
  name: 'ProjectsSection',
  data() {
    return {
      projects: [
        {
          icon: '🎮',
          title: 'Simple 3D Graphics game with Three.js',
          description: 'An implementation of the board game (Othello) playable against an AI using the MinMax algorithm enhanced with Alpha-Beta pruning. The game was developed in JavaScript with the help of the Three.js library for graphical visualization of the game board.',
          githublink: 'https://github.com/bycrn/PROJET-Othello',
          technologies: ['JavaScript', 'Three.js', '3D Graphics', 'WebGL', 'MinMax Algorithm', 'Alpha-Beta Pruning']
        },
        {
          icon: '🚇',
          title: 'Metro-Bellman-Ford: Paris Metro Route Planner',
          description: 'A Python application implementing the Bellman-Ford algorithm to calculate optimal routes in the Paris metro network. The program features a Tkinter-based GUI that enables users to visualize and navigate the metro system efficiently, finding the shortest path between any two stations while accounting for travel time.',
          githublink: 'https://github.com/bycrn/Graph-explorer',
          technologies: ['Python', 'Tkinter (GUI)', 'Bellman-Ford Algorithm', 'Graph Theory', 'Data Structures']
        },
        {
          icon: '💻',
          title: 'Turing Machine Simulator',
          description: 'Python implementation of a step-by-step execution simulation of a Turing machine with linker functionality and no graphical interface. The project was coded using Object-Oriented Programming (OOP) principles in Python. Text files were used to describe the Turing machines, and a linker function was created to call other machines (in the form of .txt files).',
          githublink: 'https://github.com/bycrn/Projet-Theorie-des-langages',
          technologies: ['Python', 'OOP', 'Text Files']
        }
      ]
    }
  }
}
</script>