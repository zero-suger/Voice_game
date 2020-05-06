<template>
  <div class="appFooter">
      <footer class="footer mt-auto py-3 btn-primary fixed-bottom">
          <div class="container">
          <p class="text-center">&copy;{{title}}</p>
          </div>
      </footer>
  </div>
</template>

<script>
export default {
  name: 'appFooter',
  data(){
      return{
          title:"Copyright 2020. Urinov Azizbek"
      }
  }

}
</script>


<style scoped>
p{
    font-weight: bold;
    font-size: 18px;
    color: white;
}

</style>
