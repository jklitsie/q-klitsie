<template>
  <q-page>

    <!--    <q-btn @click="randomize" />-->
    <div class="row">
      <div class="q-mr-auto col-lg-4 col-sm-12">
        <h2>Wat doe ik nu</h2>
        <span>Op dit moment bevind ik me in het laatste jaar van mijn studie Software Engineering aan de Hogeschool van Amsterdam, en ben ik werkzaam bij
          <a href="http://mccs.nl" target="_blank">MCCS</a> te Almere</span>
      </div>
      <div class=" col-sm-12 col-lg-7">
        <h2>Wat kan ik</h2>
        <div class="q-mb-md">
          <div class="chevron"><strong>Talen</strong></div>
          <div class="chevron">Java</div>
          <div class="chevron">Php</div>
          <div class="chevron">HTML&CSS</div>
          <div class="chevron">Javascript</div>
          <div class="chevron">Bash</div>
        </div>
        <div class="q-mb-md">
          <div class="chevron"><strong>Frameworks</strong></div>
          <div class="chevron">Maven</div>
          <div class="chevron">Laravel</div>
          <div class="chevron">Vue & React</div>
          <div class="chevron">Typescript</div>
        </div>
        <div class="q-mb-md">
          <div class="chevron"><strong>Data</strong></div>
          <div class="chevron">MySQL</div>
          <div class="chevron">Redis</div>
          <div class="chevron">MongoDB</div>
        </div>
        <div class="q-mb-md">
          <div class="chevron"><strong>Methoden</strong></div>
          <div class="chevron">Agile</div>
          <div class="chevron">Scrum</div>
          <div class="chevron">MVC</div>
        </div>
        <!--        <span>Java</span>-->
        <!--        <q-linear-progress :value="skills.php" color="white" class="q-mt-sm" />-->
        <!--        <span>Php</span>-->
        <!--        <q-linear-progress :value="skills.php" color="white" class="q-mt-sm" />-->
        <!--        <span>Vue</span>-->
        <!--        <q-linear-progress :value="skills.vue" color="white" class="q-mt-sm" />-->
        <!--        <span>React</span>-->
        <!--        <q-linear-progress :value="skills.react" color="white" class="q-mt-sm" />-->
        <!--        <span>MySQL</span>-->
        <!--        <q-linear-progress :value="skills.mysql" color="white" class="q-mt-sm" />-->
        <!--        <span>Redis</span>-->
        <!--        <q-linear-progress :value="skills.redis " color="white" class="q-mt-sm" />-->
      </div>
    </div>

    <div class="row">
      <div class="col">
        <h2>Wat heb ik gedaan </h2>
      </div>
    </div>
    <div class="row previous-exp">
      <q-card class="my-card col-lg-4 col-xs-12 bg-secondary text-white q-mr-sm q-mt-md" :class="{activated: expand}">
        <q-card-section class="flex justify-between card-head">
          <div class="text-h6">
            <a href="https://github.com" target="_blank"><strong>Permissions API</strong></a>
            <br>
            <p class="text-subtitle1">2022-2021</p>
          </div>
          <div class="icon-container">
            <q-icon name="mdi-docker"/>
            <q-icon name="mdi-language-javascript"/>
            <q-icon name="mdi-vuejs"/>
            <q-icon name="mdi-language-php"/>
            <q-icon name="mdi-laravel"/>
          </div>
        </q-card-section>

        <q-card-section class="flex justify-between card-bottom-col" v-if="!expand">
          <div class="col-6 short-text">Tijdens mijn verdiepings semester voor mijn Software Engeering opleiding kregen
            wij de kans om een eigen project te definiëren en op te zetten.
            Hiervoor hebben wij gekozen om een dynamische authenticatie middleware te schrijven.
          </div>
          <div class="col-6 dropdown-toggle">
            <q-icon @click="this.expand = !this.expand" name="expand_more" size="1.5rem"/>
          </div>
        </q-card-section>
        <q-card-section class="flex justify-between card-bottom-exp" v-if="expand">
          <div class="col-6">Tijdens mijn verdiepings semester voor mijn Software Engeering opleiding kregen wij de kans
            om een eigen project te definiëren en op te zetten.
            Hiervoor hebben wij gekozen om een dynamische authenticatie middleware te schrijven. In de middleware bevond
            zich een authenticatie laag voor administrators en gebruikers. De administrators hadden de mogelijkheid om
            uitgaande API's en routes te registreren en die beschikbaar te stellen voor gebruikers.
            <br><br>
            We hebben het front-end opgezet in Vue3 en Quasar, de backend bestaat uit PHP8 en Laravel. Daarnaast hebben
            we veel tijd gespendeerd om de automatiseringstraat binnen gitlab aan het werk te krijgen. Hiervoor hebben
            we gebruik gemaakt van een docker solution waarmee we de kwaliteit en deployement konden verifiëren en
            automatiseren.
          </div>
          <div class="col-6 dropdown-toggle">
            <q-icon @click="this.expand = !this.expand" name="expand_less" size="1.5rem"/>
          </div>
        </q-card-section>

      </q-card>

      <q-card class="my-card col-lg-4 col-xs-12 bg-secondary text-white  q-mr-sm q-mt-md" :class="{activated: expand2}">
        <q-card-section class="flex justify-between card-head">
          <div class="text-h6">
            <a href="https://www.graylog.org/" target="_blank"><strong>Graylog Automatisering</strong></a>
            <br>
            <p class="text-subtitle1">2022-2021</p>
          </div>
          <div class="icon-container">
            <q-icon name="mdi-powershell"/>
            <q-icon name="mdi-language-python"/>
          </div>
        </q-card-section>

        <q-card-section class="flex justify-between card-bottom-col" v-if="!expand2">
          <div class="col-6 short-text">Tijdens mijn stage bij Defensie heb ik de opdracht gekregen om een implimentatie
            van het open source software project genaamd Graylog uit te breiden met een automatiserings functionaliteit
            die ervoor zorgt dat scraped data gesynchroniseerd wordt.
          </div>
          <div class="col-6 dropdown-toggle">
            <q-icon @click="this.expand2 = !this.expand2" name="expand_more" size="1.5rem"/>
          </div>
        </q-card-section>
        <q-card-section class="flex justify-between card-bottom-exp" v-if="expand2">
          <div class="col-6">Tijdens mijn stage bij Defensie heb ik de opdracht gekregen om een implimentatie van het
            open source software project genaamd Graylog uit te breiden met een automatiserings functionaliteit die
            ervoor zorgt dat scraped data gesynchroniseerd wordt. <br><br> Hiervoor moest er gebruik gemaakt worden van
            meerdere Powershell scripten die aangesproken werden door een overkoepelend Python functionaliteit. De data
            werd daarna gebundeld en naar een centrale opslag gestuurd om uitgelezen te worden en te synchroniseren met
            de Graylog API.
          </div>
          <div class="col-6 dropdown-toggle">
            <q-icon @click="this.expand2 = !this.expand2" name="expand_less" size="1.5rem"/>
          </div>
        </q-card-section>

      </q-card>

      <q-card class="my-card col-lg-4 col-xs-12 bg-secondary text-white q-mt-md" :class="{activated: expand3}">
        <q-card-section class="flex justify-between card-head">
          <div class="text-h6">
            <a href="weedportal.com" target="_blank"><strong>Weedportal</strong></a>
            <br>
            <p class="text-subtitle1">2019</p>
          </div>
          <div class="icon-container">
            <q-icon name="mdi-language-javascript"/>
            <q-icon name="mdi-vuejs"/>
            <q-icon name="mdi-language-html5"/>
            <q-icon name="mdi-language-php"/>
            <q-icon name="mdi-laravel"/>
          </div>
        </q-card-section>

        <q-card-section class="flex justify-between card-bottom-col" v-if="!expand3">
          <div class="col-6 short-text">Tijdens mijn eindstage tijdens mijn studie Applicatie-Ontwikkelaar heb ik meegewerkt aan
            het project Weedportal</div>
          <div class="col-6 dropdown-toggle">
            <q-icon @click="this.expand3 = !this.expand3" name="expand_more" size="1.5rem"/>
          </div>
        </q-card-section>
        <q-card-section class="flex justify-between card-bottom-exp" v-if="expand3">
          <div class="col-6">Tijdens mijn eindstage tijdens mijn studie Applicatie-Ontwikkelaar heb ik meegewerkt aan
            het project Weedportal, de visie van dit project was nieuw platform opbouwen waar gebruikers ervaringen
            konden delen over het groeien van cannabis planten. Hiervoor had het team vrije hand gekregen om zelf te
            bouwstenen te selecteren om dit in op te bouwen, er is voor gekozen om de front end in Vue2 te doen en een
            PHP backend i.c.m. Laravel.
            <br><br>
            Ik heb samengewerkt aan het implementeren van een chat systeem d.m.v. Socket.io en Redis te implementeren.
            Hier hebben we meerdere prototypes mee opgeleverd
          </div>
          <div class="col-6 dropdown-toggle">
            <q-icon @click="this.expand3 = !this.expand3" name="expand_less" size="1.5rem"/>
          </div>
        </q-card-section>

      </q-card>
    </div>
  </q-page>
</template>

<script>
import {defineComponent} from "vue";
import {ref} from 'vue'

export default defineComponent({
  name: "portfolio",
  setup() {
    const progress = ref(0.8)
    return {
      progress,
      randomize() {
        progress.value = Math.random()
      },
    }
  },
  data() {
    let expand = false;
    let expand2 = false;
    let expand3 = false;
    return {
      skills: {
        php: 0.8,
        java: 0.6,
        html: 0.9,
        vue: 0.6,
        react: 0.4,
        mysql: 0.8,
        redis: 0.2,

      },
      expand,
      expand2,
      expand3,
    }
  }
});
</script>
<style lang="scss">
@media only screen and (min-width: 1440px) {
  .previous-exp {
    flex-wrap: nowrap;
  }
}

.short-text {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.icon-container {
  line-height: 2rem;
}

.icon-container i {
  font-size: 1.5rem;
}

.my-card {
  max-height: 150px;
}

.my-card.activated {
  max-height: 1000px;
}

.card-head {
  padding-bottom: 0;
}

.card-bottom-col {
  padding-top: 0;
  margin-top: 0;
}

.card-bottom-exp {
  padding-top: 0;
  margin-top: 0;
}

.chevron {
  color: white;
  display: inline-block;
  min-width: 125px;
  text-align: center;
  padding: 8px 5px;
  margin-right: -15px;
  background: rgb(63, 63, 63);
  -webkit-clip-path: polygon(0 0, 80% 0, 100% 50%, 80% 100%, 0 100%, 20% 50%);
  clip-path: polygon(0 0, 80% 0, 100% 50%, 80% 100%, 0 100%, 20% 50%);
}

.chevron:first-child {
  color: white;
  font-size: 16px;
  display: inline-block;
  min-width: 150px;
  text-align: center;
  padding: 15px 0;
  margin-right: -15px;
  background: rgb(63, 63, 63);
  -webkit-clip-path: polygon(0 0, 76% 0, 100% 52%, 78% 100%, 0 100%, 20% 50%);
  clip-path: polygon(0 0, 76% 0, 100% 52%, 78% 100%, 0 100%, 20% 50%);
}

.dropdown-toggle {
  cursor: pointer;
}

.dropdown-toggle:hover {
  background: rgb(47, 47, 47);
  -webkit-transition: background .5s; /* For Safari 3.0 to 6.0 */
  transition: background .5s; /* For modern browsers */
}

@keyframes fadeInOpacity {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

h2 {
  margin-top: 25px;
  margin-bottom: 25px;
}
</style>
