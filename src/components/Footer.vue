<template>
  <footer>
    <p>{{copyright}} @{{title}}</p>
  </footer>
</template>

<script>
// Event Bus
import {bus} from '../main.js';

export default {
  props: {
    title: {
      type: String
    }
  },
  data () {
    return {
      copyright: 'copyright'
    }
  },
  methods: {
  },
  created(){
    bus.$on('titleChanged', (data)=>{
      this.title = data;
    })
  }
}
</script>
<style lang="stylus" scoped>
footer{
  background : #222;
  padding: 6px;
}

p {
  color: lightgreen;
  text-align: center
}
 
</style>