<template>
  <div>
    <form-helper>
      <div slot="form-header">
        <h3>This is the title of the form</h3>
        <p> Information about the form</p>
      </div>
      <div slot="form-fields">
        <input type="text" placeholder="name" required></input>
        <input type="password" placeholder="password" required></input>
      </div>
      <div slot="form-controls">
        <button @click="handleSubmit">Submit</button>
      </div>
    </form-helper>
  </div>
</template>

<script>
import formHelper from './components/formHelper.vue'
export default {
  components: {
    'form-helper': formHelper
  },
  data () {
    return {
      title: "I am a dynamic slot title"
    }
  },
  methods: {
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
