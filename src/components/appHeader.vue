<template>
  <div class="appHeader">
      <h1 class="btn-primary text-center">{{title}}</h1>
  </div>
</template>

<script>
export default {
  name: 'appHeader',
  data(){
      return{
          title:"Welcome to the CodingNewBie"
      }
  },
  methods:{
      
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
    padding: 25px;
    font-weight: bold;
    color:white;
}




</style>
