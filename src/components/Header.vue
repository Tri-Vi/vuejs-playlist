<template>
  <header>
    <h1 @click="changeTitle">{{title}}</h1>
  </header>
</template>

<script>
// Event Bus
import {bus} from '../main.js';

export default {
  components: {

  },
  props: {
    title: {
      type: String
    }
  },
  data () {
    return {
      title: 'Vue Ninjas'
    }
  },
  methods: {
    changeTitle(){
      //this.$emit('changeTitle', 'Vue Wizards');
      this.title = 'Vue Wizards';
      bus.$emit('titleChanged', 'Vue Wizards');
    }
  }
}
</script>
<style lang="stylus" scoped>
header{
  background : lightgreen;
  padding: 10px;
}

h1 {
  color: #222;
  text-align: center
}
 
</style>