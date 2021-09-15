<template>
  <section class="projects">
      <ProjectCard :item="project" v-for="project in projects" :key="project.title" />
  </section>
</template>

<script>
export default {
data() {
    return {
      projects: [
        {
          // image: require('~/assets/images/giphy.png'),
          title: 'Giphy Search',
          description: 'A web app that allows users to search their favorite gifs, copy the url, and use at their own discretion',
          tech: 'HTML, CSS, SCSS, JS',
          source: 'https://github.com/daystone4/Giphy-Search',
          link: 'https://search-giphy-app.netlify.app/',
        },
        {
          // image: require('~/assets/images/splitter.png'),
          title: 'Splitter',
          description: 'A Frontend Mentor project that allows users to calculate individual tip amounts for a shared bill',
          tech: 'HTML, CSS, JS',
          source: 'https://github.com/daystone4/frontendmentor-splitter-app',
          link: 'https://frontendmentor-splitter.netlify.app/',
        },
        {
          // image: require('~/assets/images/filter.png'),
          title: 'User Filter',
          description: 'A web app that filters through a random list of users based on text that is inputted into the search field',
          tech: 'HTML, CSS, JS',
          source: 'https://github.com/daystone4/user-filter',
          link: 'https://filter-users.netlify.app/'
        },
        {
          // image: require('~/assets/images/filter.png'),
          title: 'Quiz App',
          description: 'This web app allows users to take a short quiz and save their high scores to local storage',
          tech: 'HTML, CSS, JS',
          source: 'https://github.com/daystone4/quiz-app',
          link: 'https://fast-quiz.netlify.app/',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.projects {
    margin: 6rem 0 0;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5em;
}
</style>