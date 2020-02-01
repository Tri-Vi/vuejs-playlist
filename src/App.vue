<template>
  <div>
    <app-header v-bind:title="title" v-on:changeTitle="udpateTitle($event)"></app-header>
    <app-ninjas v-bind:ninjas="ninjas"></app-ninjas>
    <app-footer v-bind:title="title"></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Ninjas from './components/Ninjas.vue'

export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'app-ninjas': Ninjas
  },
  data () {
    return {
      ninjas: [
        {id: 1, name: 'Ryu', speciality: 'Vue Components', show: false},
        {id: 2, name: 'Crystal', speciality: 'HTML Wizardy', show: false},
        {id: 3, name: 'Hitoshi', speciality: 'Click Events', show: false},
        {id: 4, name: 'Tango', speciality: 'Conditionals', show: false},
        {id: 5, name: 'Kami', speciality: 'Webpack', show: false},
        {id: 6, name: 'Yoshi', speciality: 'Data Design', show: false}
      ],
      title: "Vue Title"
    }
  },
  methods: {
    udpateTitle(e){
      this.title = e;
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}
</style>
