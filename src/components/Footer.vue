<template>
  <footer>
    <p>{{copyright}}</p>
  </footer>
</template>

<script>

export default {
  data () {
    return {
      copyright: 'copyright @tv'
    }
  },
  methods: {
    
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