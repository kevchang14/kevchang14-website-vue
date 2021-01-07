<template>
  <div id="app">
    <NavBar />
    <IntroductionBanner />
    <AboutMe />
    <PersonalProjects />
    <!--<HelloWorld v-bind:msg="msg" v-bind:id="1" />
    <GroceryList v-bind:list="groceryList" />-->
  </div>
</template>

<script>
//Keep these two components and associated code to show how data can be passed between components
//import HelloWorld from './components/HelloWorld.vue'
//import GroceryList from './components/GroceryList.vue'
import NavBar from './components/NavBar.vue'
import IntroductionBanner from './components/IntroductionBanner.vue'
import AboutMe from './components/AboutMe.vue'
import PersonalProjects from './components/PersonalProjects.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    IntroductionBanner,
    AboutMe,
    PersonalProjects
    //HelloWorld,
    //GroceryList,
  },
  /*data: () => {
    return {
      msg: "Welcome to Your Vue.js App Kevin",
      groceryList: [
        { id: 0, text: 'Vegetables' },
        { id: 1, text: 'Cheese' },
        { id: 2, text: 'Whatever else humans are supposed to eat' }
      ]
    }
  }*/
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
}
</style>
