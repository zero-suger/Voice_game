<template>
  <div class="appIndex container border border-primary">
    
    <div class="row" >
        <div class="col cat " data-toggle="tooltip" data-placement="top" title="Cat">
             <img @click="availableCat = !availableCat"  alt="Cat" src="@/assets/img/cat.png">
             <div v-if = "availableCat">
                  <audio src="@/assets/sounds/cat.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Lion">
             <img @click="availableLion = !availableLion"  alt="Lion" src="@/assets/img/lion.png">
    
             <div v-if = "availableLion">
                  <audio src="@/assets/sounds/lion.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Horse">
             <img @click="availableHorse = !availableHorse"  alt="Horse" src="@/assets/img/horse.png">
    
             <div v-if = "availableHorse">
                  <audio src="@/assets/sounds/horse.mp3" autoplay/>
             </div>
        </div>
    </div> 
    <div class="row">
        <div class="col" data-toggle="tooltip" data-placement="top" title="Duck">
             <img @click="availableDuck = !availableDuck"  alt="Duck" src="@/assets/img/duck.png">
             <div v-if = "availableDuck">
                  <audio src="@/assets/sounds/duck.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Cock">
             <img @click="availableCock = !availableCock"  alt="Cock" src="@/assets/img/cock.png">
    
             <div v-if = "availableCock">
                  <audio src="@/assets/sounds/cock.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Dog">
             <img @click="availableDog = !availableDog"  alt="Dog" src="@/assets/img/dog.png">
    
             <div v-if = "availableDog">
                  <audio src="@/assets/sounds/dog.mp3" autoplay/>
             </div>
        </div>
    </div> 
  </div>
</template>

<script>
export default {
  name: 'animalsVoice',
  data(){
      return{
          availableCat:false,
          availableLion:false,
          availableHorse:false,
          availableDuck:false,
          availableDog:false,
          availableCock:false,
          
      }
  }
}


</script>


<style scoped >
.row {
    padding-bottom: 50px ;
}
img{
    height: 200px;
}
.appIndex{
    margin-top:20px; 
    margin-bottom:20px; 
    padding: 30px;
    
}
</style>
