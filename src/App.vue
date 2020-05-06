<template>
  <div id="app">
   
    <appHeader/>
    <div class="text-center">
      <!-- Button trigger modal -->
<button type="button" class="btn btn-danger btn-outline-primary" data-toggle="modal" data-target="#exampleModal">
  Simple Game Rules <i class="fas fa-exclamation-triangle"></i>
</button>
  </div>
<!-- Modal -->
<div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel" style="font-weight:bold;">Welcome to the simple Voice Listening Game.</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <br> There are total 3 options: Human voices, Animal voices and Musical instrument voices. <br> <br> <span style="color:red; font-weight:bold; font-size:18px;">Choose one and click 1 time to listen and click 1 time to stop listening.</span>
        <br> <br>  Good Luck!  
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-primary" data-dismiss="modal">Close</button>
        
      </div>
    </div>
  </div>
</div>
        <!-- <button @click="readRules" class="btn btn-lg btn-danger btn-outline-primary">Click me to see game rules. <i class="fas fa-exclamation-triangle"></i></button> -->
    
    <div class="text-center menu">
      <component v-bind:is="component"></component>
      <button class="btn btn-lg btn-danger btn-outline-primary" v-on:click="component = 'animalsVoice'">Show Animal Voices <i class="fas fa-paw"></i></button>
      <button class="btn btn-lg btn-danger btn-outline-primary" v-on:click="component = 'peopleVoices'">Show Human voices <i class="fas fa-user"></i></button>
      <button class="btn btn-lg btn-danger btn-outline-primary" v-on:click="component = 'instrumentVoices'">Show instrument Voices <i class="fas fa-music"></i></button>
    </div>
    <appIndex/>
    <appFooter/>
    
    
  </div>
</template>

<script>
import appHeader from './components/appHeader.vue'
import appIndex from './components/appIndex.vue'
import appFooter from './components/appFooter.vue'
import animalsVoice from './components/animalsVoice.vue'
import peopleVoices from './components/peopleVoices.vue'
import instrumentVoices from './components/instrumentVoices.vue'

export default {
  name: 'App',
  
  components: {
    appHeader,
    appFooter,
    appIndex,
    animalsVoice,
    peopleVoices,
    instrumentVoices,
  },
  data(){
    return{
      component:'animalsVoice'
    }
  },
  methods:{
      // readRules: function(){
      //     alert("This is a simple game. Click each animal picture to listen each animal voice. Click one time to listen and click one time to stop!")
      // }
  }
}
</script>

<style scoped>
.menu{
  padding: 20px;
  margin-bottom:100px ;
  
}
button{
  margin: 5px;
  color: white;
}
</style>
