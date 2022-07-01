<template>
  <q-page>

<!--    <q-btn @click="randomize" />-->
    <div class="row">
      <div class="q-ma-md col">
        <h2>Waar ben ik nu te vinden</h2>
        <span>Het moet lekker werken, Dat is mijn motto. Ik ben een leergierige developer die zich altijd verdiept in nieuw en oud. Een nonchalant iemand die altijd zoekt naar de best passende oplossing voor elk probleem of vraag.
          Laat wat van je horen dan kan ik misschien spoedig iets voor jou betekenen</span>s
      </div>
      <div class="q-ma-md col">
        <h2>Skills</h2>
        <span>Java</span>
        <q-linear-progress :value="skills.php" color="white" class="q-mt-sm" />
        <span>Php</span>
        <q-linear-progress :value="skills.php" color="white" class="q-mt-sm" />
        <span>Vue</span>
        <q-linear-progress :value="skills.vue" color="white" class="q-mt-sm" />
        <span>React</span>
        <q-linear-progress :value="skills.react" color="white" class="q-mt-sm" />
        <span>MySQL</span>
        <q-linear-progress :value="skills.mysql" color="white" class="q-mt-sm" />
        <span>Redis</span>
        <q-linear-progress :value="skills.redis " color="white" class="q-mt-sm" />
      </div>
    </div>
    <div class="row">
      <div class="q-ma-md col">
        <h1>Latest collaberations & employement</h1>
      </div>
    </div>
    <div class="row">
      <q-card class="my-card col bg-secondary text-white q-ma-md">
        <q-card-section class="flex justify-between">
          <div class="text-h6">Internship at the ministery of defense</div>
          <div class="icon-container">
            <q-icon name="mdi-vuejs" />
            <q-icon name="mdi-language-html5" />
          </div>
          <div class="text-subtitle2">Timeframe</div>
        </q-card-section>

        <q-card-section class="row">
          <div class="col-6">asd</div>
          <div class="col-6">
            <q-img src="../assets/bg.jpg" />
          </div>
        </q-card-section>

        <q-separator color="white" />

        https://mxb.dev/
      </q-card>

      <q-card class="my-card col bg-secondary text-white q-ma-md">
        <q-card-section>
          <div class="text-h6">Our Changing Planet</div>
          <div class="text-subtitle2">by John Doe</div>
        </q-card-section>

        <q-card-section>
          asdasd a
        </q-card-section>

        <q-separator dark />

        <q-card-actions>
          <q-btn flat>Action 1</q-btn>
          <q-btn flat>Action 2</q-btn>
        </q-card-actions>
      </q-card>

      <q-card class="my-card col bg-secondary text-white q-ma-md">
        <q-card-section class="flex justify-between">
          <div class="text-h6">Weedportal</div>
          <div class="icon-container">
            <q-icon name="mdi-vuejs" />
            <q-icon name="mdi-language-html5" />
            <q-icon name="mdi-language-php" />
          </div>
        </q-card-section>

        <q-card-section class="row">
          <div class="col-6">asd</div>
          <div class="col-6">
            <q-img src="../assets/bg.jpg" />
          </div>
        </q-card-section>

        <q-separator color="white" />

      </q-card>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import { ref } from 'vue'
export default defineComponent({
  name: "portfolio",
  setup () {
    const progress = ref(0.8)
    return {
      progress,
      randomize () {
        progress.value = Math.random()
      }
    }
  },
  data(){
    return {
      skills: {
        php: 0.8,
        java: 0.6,
        html: 0.9,
        vue: 0.6,
        react: 0.4,
        mysql: 0.8,
        redis: 0.2,

      }
    }
  }
});
</script>
<style lang="scss">
.icon-container {
  line-height:2rem;

}
</style>
