<template>
  <div>
    <app-header></app-header>
    <router-view></router-view>
    <!-- <show-blog></show-blog> -->
    <!-- <list-blog></list-blog> -->
    <!-- <add-blog></add-blog> -->
  </div>
</template>

<script>
import addBlog from './components/addBlog.vue';
import showBlog from './components/showBlog.vue';
import listBlog from './components/listBlog.vue';
import header from './components/header.vue';

export default {
  components: {
    'add-blog': addBlog,
    'show-blog': showBlog,
    'list-blog': listBlog,
    'app-header': header
  },
  data () {
    return {
      
    }
  },
  methods: {
    
  }
}
</script>

<style>
body{
    margin: 0;
    font-family: 'Nunito SemiBold';
}
</style>
