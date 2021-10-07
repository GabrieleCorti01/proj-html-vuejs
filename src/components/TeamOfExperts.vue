<template>
  <div class="container-fluid pt-5">
      <div class="row justify-content-center p-5">
    <!-- Team con i vari oogetti a sinistra -->
           <div class="col-4" id="team-container">
               <p class="upper-title">WE LIKE WHAT WE DO</p>
               <span class="bg-text-white me-2">Team</span><span>of Experts</span>
               <p class="subtitle-main mt-3">Ethics and integrity are the bases on which ourprofessionals build their careers. They are fundamentals that become daily attitudes.</p>
    <!-- Sezione interna con all'interno i vari membri del team -->
               <div class="row mt-5">
                   <TeamElement class="col-5 mb-5" v-for="(element, index) in teamElement" :key="index" :name="element.name" :source="element.src" :subtitle="element.subtitle"/>
               </div>
           </div>

    <!-- Discorso del presidente a destra -->
           <div class="col-2" id="speech-container">
               <h4 class="mb-3">President Speech</h4>
               <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Numquam ipsa doloribus modi fuga</p> 
               <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia atque rerum, pariatur ipsum nam dolor nulla quibusdam, harum laboriosam corporis, facilis totam? Et inventore at assumenda sed delectus facere dolores.</p>
               <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nemo iste neque sit vel provident ex.</p>
               <span>T.Johnson</span><span><i class="fas fa-quote-right"></i></span>
           </div>
      </div>
  </div>
</template>

<script>
import TeamElement from './TeamElement.vue'
import teamElement from '../data/teamElement'

export default {
name: 'TeamOfExperts',
components: {
    TeamElement,
},
data : function (){
    return {
        teamElement
    }
}

}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

#team-container{
    span{
        font-size: 2.8em;
        font-weight: 700;
    }
}

#speech-container{
    background-color: $primaryColor;
    padding: 30px;
    border-radius: 10px;
    h4{
        font-weight: 700;
    }
    p{
        font-weight: 300;
        font-size: 0.9em;
    }
    i{
        color: rgb(3, 80, 80);
        padding-left: 150px;
    }
}

.container-fluid{
    background-color: $secondaryColor;
    color: white;
}

</style>