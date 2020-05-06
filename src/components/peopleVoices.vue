<template>
  <div class="appIndex container border border-primary">
    
    <div class="row" >
        <div class="col " data-toggle="tooltip" data-placement="top" title="Baby Cry">
             <img @click="availableBaby_cry = !availableBaby_cry"  alt="Baby Cry" src="@/assets/img/baby_cry.png">
             <div v-if = "availableBaby_cry">
                  <audio src="@/assets/sounds/baby_cry.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Cough">
             <img @click="availableCough = !availableCough"  alt="Cough" src="@/assets/img/cough.png">
    
             <div v-if = "availableCough">
                  <audio src="@/assets/sounds/cough.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Farting">
             <img @click="availableFarting = !availableFarting"  alt="Farting" src="@/assets/img/farting.png">
    
             <div v-if = "availableFarting">
                  <audio src="@/assets/sounds/farting.mp3" autoplay/>
             </div>
        </div>
    </div>
    <div class="row" >
        <div class="col " data-toggle="tooltip" data-placement="top" title="Snoring">
             <img @click="availableSnoring = !availableSnoring"  alt="Snoring" src="@/assets/img/snoring.png">
             <div v-if = "availableSnoring">
                  <audio src="@/assets/sounds/snoring.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Shouting">
             <img @click="availableShouting = !availableShouting"  alt="Shouting" src="@/assets/img/shouting.png">
    
             <div v-if = "availableShouting">
                  <audio src="@/assets/sounds/shouting.mp3" autoplay/>
             </div>
        </div>
        <div class="col" data-toggle="tooltip" data-placement="top" title="Heartbeating">
             <img @click="availableHeartbeating = !availableHeartbeating"  alt="Heartbeating" src="@/assets/img/heartbeating.png">
    
             <div v-if = "availableHeartbeating">
                  <audio src="@/assets/sounds/heartbeat.mp3" autoplay/>
             </div>
        </div>
    </div>  
    
  </div>
</template>

<script>
export default {
  name: 'peopleVoices',
  data(){
      return{
          availableBaby_cry:false,
          availableCough:false,
          availableFarting:false,
          availableSnoring:false,
          availableShouting:false,
          availableHeartbeating:false,
          
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
