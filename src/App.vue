<template>
  <div>
  
    <show-blog></show-blog>
    <list-blog></list-blog>
    <!--
   <add-blog></add-blog>
    -->
  </div>
</template>

<script>
import addBlog from './components/addBlog.vue';
import showBlog from './components/showBlog.vue';
import listBlog from './components/listBlog.vue';

export default {
  components: {
    'add-blog': addBlog,
    'show-blog': showBlog,
    'list-blog': listBlog
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
