<template>
  <div>
    <the-header title="Remember Me"></the-header>
    <stored-resources :resources="storedResources" />
    <button>Enter</button>
  </div>
</template>

<script>
import StoredResources from './components/Resources/StoredResources.vue';
import TheHeader from './components/layout/TheHeader.vue';

export default {
  components: {
    StoredResources,
    TheHeader
  },
  data() {
    return {
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official guide',
          description: 'The Official Vue.js documentation.',
          link: 'https://vuejs.org'
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn to google...',
          link: 'https://google.com'
        },
        {
          id: 'youtube',
          title: 'Youtube',
          description: 'Learn from videos, use Youtube.',
          link: 'https://youtube.com'
        }
      ]
    };
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
