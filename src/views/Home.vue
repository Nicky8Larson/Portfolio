<template>
  <v-app
    id="home"
    :style="{ background: $vuetify.theme.themes.dark.background }"
  >
    <nav-bar />
    <v-container fluid>
      <v-row>
        <v-col cols="6">
          <v-img src="1.png" contain max-height="500" class="ml-15 mr-15 mt-5" id="imgSmy"></v-img>
        </v-col>
        <v-col cols="6">
          <h5 class="blue--text text--darken-3 top">Bonjour, je suis</h5>
          <h1 class="white--text">Sammy Merazga</h1>
          <p class="grey--text">
            Je suis un étudiant en Bac +3 à l'<a
              href="https://www.institut-g4.fr/"
              class="text-decoration-none"
              >Institut G4</a
            >
            qui est une école <br />qui nous forme à une double compétence en
            informatique et en management.
          </p>
          <p class="grey--text">
            J'effectue ma poursuite d'études en alternance avec l'entreprise
            <a href="https://www.tempo-one.com/" class="text-decoration-none"
              >Tempo One</a
            >
            <br />
            en tant que développeur Full Stack.
          </p>
          <v-btn href="../assets/others/CV.pdf" target="_blank" tile color="#2465aa" dark>Mon CV</v-btn>
        </v-col>
        <v-col cols="12" class="padd">
          <div class="first" id="skills">
            <v-row>
              <v-col cols="12">
                <div class="child bgColor1 mr-5" id="shadow">
                  <v-icon color="#2465aa" x-large class="ml-3"
                    >fas fa-desktop</v-icon
                  >
                  <h3 class="white--text ml-3 mt-4">Back-end</h3>
                  <p class="grey--text ml-3 mt-6">
                    <ul>
                      <li>NodeJS</li>
                      <li>Express.js</li>
                      <li>Symfony</li>
                    </ul>
                  </p>
                <v-dialog v-model="dialogBackEnd" persistent width="600px">
                <template v-slot:activator="{ on, attrs }">
                  <v-btn color="#2465aa" dark text v-bind="attrs" v-on="on">
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                  </template>
                  <v-card color="#181818" class="rounded-xl">
                    <v-card-title class="justify-center text-center">
                      <span class="text-h5 blue--text text-decoration-underline">Back-end</span>
                    </v-card-title>
                    <v-card-text class="text-center white--text mt-2">
                      <p>Je suis en capacité de développer un back-end en NodeJS (petite préférence avec TypeScript 😅) ainsi qu'avec le framework de PHP Symfony (PHP Vanilla aussi).</p>
                      <p>Concernant les bases de données, j'ai déjà travaillé avec du PostgreSQL, MySQL, SQLite ainsi que MongoDB (NoSQL).</p>
                      <p class="caption">Je vous invite à aller sur mon Github pour voir les projets en questions avec ces technologies 😃</p>
                    </v-card-text>
                    <v-card-actions>
                    <v-btn icon href="https://github.com/SammyMERAZGA?sort=&tab=repositories" target="_blank">
                      <v-icon color="#2465aa">fab fa-github</v-icon>
                    </v-btn>
                      <v-spacer></v-spacer>
                      <v-btn color="blue darken-1" text @click="dialogBackEnd = false">
                        Retour
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-dialog>
                </div>
                <div class="child bgColor2" id="whiteShadow">
                  <v-icon x-large class="ml-3" dark
                    >fas fa-server</v-icon
                  >
                  <h3 class="white--text ml-3 mt-4">Front-end</h3>
                  <p class="white--text ml-3 mt-6">
                    <ul>
                      <li>TypeScript</li>
                      <li>VueJS</li>
                      <li>React</li>
                    </ul>
                  </p>
                  <v-dialog v-model="dialogFrontEnd" persistent width="600px">
                <template v-slot:activator="{ on, attrs }">
                  <v-btn color="white" dark text v-bind="attrs" v-on="on">
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                  </template>
                  <v-card color="#181818" class="rounded-xl">
                    <v-card-title class="justify-center text-center">
                      <span class="text-h5 blue--text text-decoration-underline">Front-end</span>
                    </v-card-title>
                    <v-card-text class="text-center white--text mt-2">
                      <p>Le front-end ce que je préfère lors du développement d'une application web 🥰.</p>
                      <p>J'utilise principalement le framework VueJS que j'apprécie énormément !</p>
                      <p class="caption">Je combine VueJS avec le langage TypeScript pour avoir plus de sécurité dans mon code et pour gagner en lisibilité. De plus, j'utilise Vuetify (Material Design Framework) car je trouve le style Material Design très beau 🤗.</p>
                      <p>Malgré ma préférence pour VueJS, je peux aussi très bien faire du React avec Material UI qui est une libraire UI (Material Design) de React fonctionnant comme Vuetify.</p>
                    </v-card-text>
                    <v-card-actions>
                    <v-btn icon href="https://github.com/SammyMERAZGA?sort=&tab=repositories" target="_blank">
                      <v-icon color="#2465aa">fab fa-github</v-icon>
                    </v-btn>
                      <v-spacer></v-spacer>
                      <v-btn color="blue darken-1" text @click="dialogFrontEnd = false">
                        Retour
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-dialog>
                </div>
                <div class="child bgColor1 ml-3" id="shadow">
                  <v-icon color="#2465aa" x-large class="ml-3"
                    >fas fa-users</v-icon
                  >
                  <h3 class="white--text ml-3 mt-4">Gestion de projet</h3>
                  <p class="grey--text ml-3 mt-6">
                    <ul>
                      <li>Jira Software</li>
                      <li>GanttProject</li>
                      <li>Microsoft Project</li>
                    </ul>
                  </p>
                  <v-dialog v-model="dialogManagement" persistent width="600px">
                <template v-slot:activator="{ on, attrs }">
                  <v-btn color="#2465aa" dark text v-bind="attrs" v-on="on">
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                  </template>
                  <v-card color="#181818" class="rounded-xl">
                    <v-card-title class="justify-center text-center">
                      <span class="text-h5 blue--text text-decoration-underline">Gestion de projet</span>
                    </v-card-title>
                    <v-card-text class="text-center white--text mt-2">
                      <p>Étant étudiant à l'Institut G4, on est formé à une double compétence à la fois en informatique mais aussi en gestion de projet .</p>
                      <p>L'école nous permet de décrocher le Titre de "Chef de Projet Système d'Information" (certifié par l'État - RNCP niveau 7).</p>
                      <p>Je suis donc en capacité de gérer un projet 😀.</p>
                    </v-card-text>
                    <v-card-actions>
                    <v-btn icon href="https://github.com/SammyMERAZGA?sort=&tab=repositories" target="_blank">
                      <v-icon color="#2465aa">fab fa-github</v-icon>
                    </v-btn>
                      <v-spacer></v-spacer>
                      <v-btn color="blue darken-1" text @click="dialogManagement = false">
                        Retour
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-dialog>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
        <v-col md="3" offset-md="3" id="about">
          <h3 class="white--text" id="project">Projets</h3>
        </v-col>
        <v-col md="3" class="text-end">
          <v-btn
            tile
            color="#2465aa"
            dark
            class="rounded-xl"
            href="https://github.com/SammyMERAZGA?tab=repositories"
            target="_blank"
          >
            Tout voir
          </v-btn>
        </v-col>
        <v-col md="3" offset-md="3">
          <v-card
            outlined
            tile
            id="shadow"
            height="230px"
            color="#1E1E1E"
          >
            <v-img src="../assets/EcoServices.png" contain></v-img>
          </v-card>
          <div class="text-center">
            <v-btn color="white" dark text class="ml-n4 mt-5 mb-2 text-decoration-underline">
              Éco Services
            </v-btn><br>
            <v-dialog v-model="dialogProject1" persistent width="600px">
                <template v-slot:activator="{ on, attrs }">
                  <v-btn color="#2465aa" dark text class="ml-n4" v-bind="attrs" v-on="on">
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                  </template>
                  <v-card color="#181818" class="rounded-xl">
                    <v-card-title class="justify-center text-center">
                      <span class="text-h5 blue--text text-decoration-underline">Éco Services</span>
                    </v-card-title>
                    <v-card-text class="text-center white--text mt-2">
                      <p>J'ai réalisé ce projet dans le cadre de mes études à l'Institut G4 🎓.</p>
                      <p>Éco Services est un site e-commerce avec la possibilité d'acheter des produits éco-responsables ainsi que de faire une demande de devis pour un service écologique.</p>
                      <p>Technologies utilisées ➡️ Front-end : TypeScript, VueJS et Vuetify | Back-end : TypeScript, NodeJS (Express), PrismaORM, PostgreSQL</p>
                    </v-card-text>
                    <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn color="blue darken-1" text @click="dialogProject1 = false">
                        Retour
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-dialog>
            <v-btn color="#2465aa" dark text class="ml-15" href="https://github.com/SammyMERAZGA/clientEcoServices" target="_blank">
              Code source <v-icon right class="mb-1">fab fa-github</v-icon>
            </v-btn>
          </div>
        </v-col>
        <v-col md="3" class="ml-5">
          <v-card
            outlined
            tile
            id="shadow"
            height="230px"
            color="#1E1E1E"
          >
            <v-img src="../assets/HealthSmy.png" contain></v-img>
          </v-card>
          <div class="text-center">
            <v-btn color="white" dark text class="ml-n4 mt-5 mb-2 text-decoration-underline">
              Health Smy
            </v-btn><br>
            <v-dialog v-model="dialogProject2" persistent width="600px">
                <template v-slot:activator="{ on, attrs }">
                  <v-btn color="#2465aa" dark text class="ml-n4" v-bind="attrs" v-on="on">
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                  </template>
                  <v-card color="#181818" class="rounded-xl">
                    <v-card-title class="justify-center text-center">
                      <span class="text-h5 blue--text text-decoration-underline">Health Smy</span>
                    </v-card-title>
                    <v-card-text class="text-center white--text mt-2">
                      <p>Il s'agit d'un projet personnel ; le projet est toujours en cours ⏳.</p>
                      <p>L'un de mes objectifs est de travailler dans la santé car c'est le domaine de mon père. J'ai donc lancé un projet dans le domaine de la santé 🏥.</p>
                      <p>Technologies utilisées : VueJS et Vuetify</p>
                    </v-card-text>
                    <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn color="blue darken-1" text @click="dialogProject2 = false">
                        Retour
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-dialog>
            <v-btn color="#2465aa" dark text class="ml-15" href="https://github.com/SammyMERAZGA/medicalDashboard" target="_blank">
              Code source <v-icon right class="mb-1">fab fa-github</v-icon>
            </v-btn>
          </div>
        </v-col>
        <v-col md="3" offset-md="3">
          <v-card
            outlined
            tile
            id="shadow"
            height="230px"
            color="white"
          >
            <v-img src="../assets/CV.png" max-height="200" class="mt-3" contain></v-img>
          </v-card>
          <div class="text-center">
            <v-btn color="white" dark text class="ml-n4 mt-5 mb-2 text-decoration-underline">
              My CV in React
            </v-btn><br>
            <v-dialog v-model="dialogProject3" persistent width="600px">
                <template v-slot:activator="{ on, attrs }">
                  <v-btn color="#2465aa" dark text class="ml-n4" v-bind="attrs" v-on="on">
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                  </template>
                  <v-card color="#181818" class="rounded-xl">
                    <v-card-title class="justify-center text-center">
                      <span class="text-h5 blue--text text-decoration-underline">Mon CV</span>
                    </v-card-title>
                    <v-card-text class="text-center white--text mt-2">
                      <p>J'ai trouvé sympa l'idée de développé un site web présentant mon CV étant donné que je suis développeur.. Puis, on économise du papier ! 💚</p>
                      <p>Technologies utilisées : React et Sass</p>
                    </v-card-text>
                    <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn color="blue darken-1" text @click="dialogProject3 = false">
                        Retour
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-dialog>
            <v-btn color="#2465aa" dark text class="ml-15" href="https://github.com/SammyMERAZGA/CV" target="_blank">
              Code source <v-icon right class="mb-1">fab fa-github</v-icon>
            </v-btn>
          </div>
        </v-col>
        <v-col md="3" class="ml-5">
          <v-card
            outlined
            tile
            id="shadow"
            height="230px"
            color="white"
          >
            <v-img src="../assets/GCR.png" max-height="200" class="mr-15 mt-5" contain></v-img>
          </v-card>
          <div class="text-center mb-15">
            <v-btn color="white" dark text class="ml-n4 mt-5 mb-2 text-decoration-underline">
              Galaxy Swiss Bourdin (GSB)
            </v-btn><br>
            <v-dialog v-model="dialogProject4" persistent width="600px">
                <template v-slot:activator="{ on, attrs }">
                  <v-btn color="#2465aa" dark text class="ml-n4" v-bind="attrs" v-on="on">
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                  </template>
                  <v-card color="#181818" class="rounded-xl">
                    <v-card-title class="justify-center text-center">
                      <span class="text-h5 blue--text text-decoration-underline">Projet GSB</span>
                    </v-card-title>
                    <v-card-text class="text-center white--text mt-2">
                      <p>J'ai réalisé ce projet dans le cadre de mon BTS SIO au lycée Victor Hugo 🎓.</p>
                      <p>Le but de ce projet était de fournir un outil informatique pour les praticiens du laboratoire GSB. (Consultation de médicaments, de praticiens et de visiteurs)</p>
                      <p>Technologies utilisées : PHP Vanilla, HTML/CSS, JavaScript, MySQL</p>
                    </v-card-text>
                    <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn color="blue darken-1" text @click="dialogProject4 = false">
                        Retour
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-dialog>
            <v-btn color="#2465aa" dark text class="ml-15" href="https://github.com/SammyMERAZGA/GCR" target="_blank">
              Code source <v-icon right class="mb-1">fab fa-github</v-icon>
            </v-btn>
          </div>
        </v-col>
      </v-row>
    </v-container>
    <Footer />
  </v-app>
</template>

<script>
import NavBar from "../components/NavBar.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "Home",
  components: {
    NavBar,
    Footer,
  },
  data () {
    return {
      dialogBackEnd: false,
      dialogFrontEnd: false,
      dialogManagement: false,
      dialogProject1: false,
      dialogProject2: false,
      dialogProject3: false,
      dialogProject4: false,
    };
  },
};
</script>

<style scoped>
.top {
  margin-top: 180px;
}
.topInverse {
  margin-top: -250px;
}
.topTolbar {
  margin-top: 100px;
  text-align: center;
}
.first {
  margin-top: 1%;
  width: 100%;
  height: 365px;
  background: linear-gradient(
    to right,
    #181818,
    #181818 50%,
    #111111 50%,
    #111111 50%
  );
  text-align: center;
  padding: 2rem 2rem;
}
.second {
  width: 100%;
  height: 400px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
}
.secondchild1 {
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-top: 250px;
}
.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}
.bgColor1 {
  background-color: #1e1e1e;
}
.bgColor2 {
  background-color: #2465aa;
}

.child1 {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  margin-right: 5px;
  width: 240px;
}
.child2 {
  display: inline-block;
  width: 245px;
  vertical-align: middle;
}
.mRight {
  margin-right: 8px;
}
.mButton {
  margin-bottom: 8px;
}
.padding {
  padding: 8px 0;
}

.col-12.padd {
  padding: 12px 0 !important;
}
.col-12.childcol {
  padding: 0 !important;
}
h1.number {
  font-size: 50px;
  font-weight: bold;
}

#imgSmy {
  border: 3px solid #2465aa;
  border-radius: 50%;
  box-shadow: #2465aa;
  box-shadow: 0 0 15px rgb(69, 144, 206);
  -webkit-transition: all 0.2s;
  -moz-transition: all 0.2s;
  -ms-transition: all 0.2s;
  -o-transition: all 0.2s;
  transition: all 0.2s;
}

#imgSmy:hover{
  transform:rotate3d(0,1,0,180deg);
}

#shadow {
  box-shadow: 0 0 15px #2465aa;
}

#whiteShadow {
  box-shadow: 0 0 15px rgb(35, 71, 187);
}
</style>
