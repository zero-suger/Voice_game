<template>
  <div class="appIndex container border border-primary">
    
    <div class="row" >
        <div class="col " data-toggle="tooltip" data-placement="top" title="Piano">
             <img @click="availablePiano = !availablePiano"  alt="Piano" src="@/assets/img/piano.png">
             <div v-if = "availablePiano">
                  <audio src="@/assets/sounds/piano.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Sitar">
             <img @click="availableSitar = !availableSitar"  alt="Sitar" src="@/assets/img/sitar.png">
    
             <div v-if = "availableSitar">
                  <audio src="@/assets/sounds/sitar.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Flute">
             <img @click="availableFlute = !availableFlute"  alt="Flute" src="@/assets/img/flute.png">
    
             <div v-if = "availableFlute">
                  <audio src="@/assets/sounds/flute.mp3" autoplay/>
             </div>
        </div>
    </div>
    <div class="row" >
        <div class="col " data-toggle="tooltip" data-placement="top" title="Trumpet">
             <img @click="availableTrumpet = !availableTrumpet"  alt="Trumpet" src="@/assets/img/trumpet.png">
             <div v-if = "availableTrumpet">
                  <audio src="@/assets/sounds/trumpet.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Guitar">
             <img @click="availableGuitar = !availableGuitar"  alt="Guitar" src="@/assets/img/guitar.png">
    
             <div v-if = "availableGuitar">
                  <audio src="@/assets/sounds/guitar.wav" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Drum">
             <img @click="availableDrum = !availableDrum"  alt="Drum" src="@/assets/img/drum.png">
    
             <div v-if = "availableDrum">
                  <audio src="@/assets/sounds/drum.mp3" autoplay/>
             </div>
        </div>
    </div>
    
    
  </div>
</template>

<script>
export default {
  name: 'instrumentVoices',
  data(){
      return{
          availablePiano:false,
          availableSitar:false,
          availableFlute:false,
          availableGuitar:false,
          availableTrumpet:false,
          availableDrum:false,
          
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
