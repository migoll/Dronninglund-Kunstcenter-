<template>
    <div>
      <div v-if="loading">Loading...</div>
      <div v-else>
        <div v-for="post in posts" :key="post.id">
          <div v-if="post.acf">
            <!-- Link to open the post in a new window using JavaScript -->
            <a href="#" @click.prevent="openPostInNewWindow(post.id)">
              <div class="udstilling-landing-page">
                <p>{{ post.acf.start_date }} <span v-if="post.acf.end_date"> - {{ post.acf.end_date }}</span></p>
                <h1>{{ post.acf.title }}</h1>
                <img :src="post.acf.image.url" alt="">
              </div>
            </a>
  
            <div class="udstilling-information">
              <h2>{{ post.acf.section_heading }}</h2>
              <div v-html="post.acf.description" class="acf-description"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        posts: [],
        loading: true
      };
    },
    methods: {
      async fetchPosts() {
        try {
          const response = await fetch('https://dronninglund-kunstcenter.laustsen.info/wp-json/wp/v2/posts?categories=5');
          const data = await response.json();
          this.posts = data;
        } catch (error) {
          console.error("Error fetching posts:", error);
        } finally {
          this.loading = false;
        }
      },
      openPostInNewWindow(postId) {
        // Open a new window and load the specific post content
        const newWindow = window.open('', '', 'width=800,height=600');
        if (newWindow) {
          // Use Nuxt.js router to navigate in the new window
          newWindow.location.href = `/udstilling/${postId}`;
        }
      }
    },
    mounted() {
      this.fetchPosts();
    }
  };
  </script>
  