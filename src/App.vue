<template>
  <div>
    <h1>{{text1}}</h1>
    <button @click="helloWorld">Click me </button>

    <p>
      <router-link to="/">Home</router-link>
      <br>
      <router-link to="/about">About</router-link>
    </p>
    <router-view></router-view>

    <Footer/>
  </div>
</template>

<script>
import Footer from './components/Footer.vue';
export default {
  data(){
    return{
      text1: 'ejemplo de texto',      
    }
  },
  components:{
    Footer,
  },
  methods:{
    helloWorld(){
      console.log('Hello world');
    }
  }

}
</script>

<style>

</style>