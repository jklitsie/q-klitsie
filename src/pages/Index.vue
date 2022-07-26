<template>
  <q-page>
      <div class=" flex row text-center banner-container banner">
        <div class="col-md-8 col-xs-12 q-pl-md q-pr-md gutter-sm text-justify">
          <h2>Welkom ik ben</h2>
          <h1>Jard Klitsie</h1>
          <h4>Software Engineer</h4>
          <div class="info">
            <span>Het moet lekker werken, dat is mijn motto. Ik ben een leergierige developer die zich altijd verdiept in nieuw en oud. Een nonchalant iemand die altijd zoekt naar de best passende oplossing voor een probleem of vraag.
          Laat wat van je <a href="https://www.linkedin.com/in/jard-klitsie-7b836b63/" target="_blank">horen</a> dan kan ik misschien spoedig iets voor jou betekenen</span>
          </div>
        </div>
        <q-avatar rounded class="col-md col-xs-0 avatar-container">
          <q-img src="~assets/j-klitsie.png"  width="75%" />
        </q-avatar>
      </div>
<!--      <div class="info row">-->
<!--        <div class="col-8 offset-4">-->
<!--        <span>Het moet lekker werken, Dat is mijn motto. Ik ben een leergierige developer die zich altijd verdiept in nieuw en oud. Een nonchalant iemand die altijd zoekt naar de best passende oplossing voor elk probleem of vraag.-->
<!--          Laat wat van je <a href="https://www.linkedin.com/in/jard-klitsie-7b836b63/" target="_blank">horen</a> dan kan ik misschien spoedig iets voor jou betekenen</span>-->
<!--        </div>-->
<!--      </div>-->
  </q-page>
</template>

<script>
import {defineComponent} from "vue";

export default defineComponent({
  name: "PageIndex",
});
</script>
<style lang="scss">
.banner-container {
  padding-top: 3em;
}
.info {
  margin: 50px 0;
  font-size: 3em;
}
.banner h1,
.banner h2,
.banner h4, {
  width: 100%;
  padding: 0px;
  margin: 0px;
  color: white;
  font-weight: 700;
}
.avatar-container .q-img {
  -webkit-clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%);
  clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%);
}
</style>
