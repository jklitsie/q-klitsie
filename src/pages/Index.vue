<template>
  <q-page>
      <div class=" flex row text-center banner-container banner">
        <q-avatar rounded class="col-md col-xs ">
          <q-img src="~assets/j-klitsie.png"  width="75%" />
        </q-avatar>
        <div class="col-md-8 col-xs-8 q-gutter-sm text-justify">
          <h2>Welkom ik ben</h2>
          <h1>Jard Klitsie</h1>
          <h4>Full stack developer</h4>
        </div>
      </div>
      <div class="info row">
        <div class="col-8 offset-4">
        <span>Het moet lekker werken, Dat is mijn motto. Ik ben een leergierige developer die zich altijd verdiept in nieuw en oud. Een nonchalant iemand die altijd zoekt naar de best passende oplossing voor elk probleem of vraag.
          Laat wat van je horen dan kan ik misschien spoedig iets voor jou betekenen</span>
        </div>
      </div>
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
.info span {
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
</style>
