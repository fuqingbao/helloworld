<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <hello-world :msg="message"/>

    <person v-for="(person, index) in persons" :person="person" :key="index"></person>
    <h1 ="TTP"></h1>

  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Person from './components/person.vue'

export default {
  name: '#app',
  components: {
    Person,
    HelloWorld
  },
  data() {
    return {
        message: '消息111',
        TTP:'你好小付',
        persons: [
          {
            name: 'zhangsan',
            gender: 'man',
            age: 24
          },
          {
            name: 'lisi',
            gender: 'man',
            age: 27
          }
        ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
