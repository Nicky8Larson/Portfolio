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
          <v-btn href="../assets/others/Merazga_Sammy_CV.pdf" target="_blank" tile color="#2465aa" dark>Mon CV</v-btn>
        </v-col>
        <v-col cols="12" class="padd">
          <div class="first" id="project">
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
                  <v-btn color="#2465aa" dark text>
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
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
                  <v-btn dark text>
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>
                <div class="child bgColor1 ml-3" id="shadow">
                  <v-icon color="#2465aa" x-large class="ml-3"
                    >fas fa-users</v-icon
                  >
                  <h3 class="white--text ml-3 mt-4">Gestion de projets</h3>
                  <p class="grey--text ml-3 mt-6">
                    <ul>
                      <li>Jira Software</li>
                      <li>GanttProject</li>
                      <li>Microsoft Project</li>
                    </ul>
                  </p>
                  <v-btn color="#2465aa" dark text>
                    En savoir plus
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
        <v-col md="3" offset-md="3" id="about">
          <h3 class="white--text">Projets</h3>
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
            <v-btn color="#2465aa" dark text class="ml-n4">
              En savoir plus <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
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
            <v-btn color="#2465aa" dark text class="ml-n4">
              En savoir plus <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
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
            <v-btn color="#2465aa" dark text class="ml-n4">
              En savoir plus <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
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
          <div class="text-center">
            <v-btn color="white" dark text class="ml-n4 mt-5 mb-2 text-decoration-underline">
              Galaxy Swiss Bourdin (GSB)
            </v-btn><br>
            <v-btn color="#2465aa" dark text class="ml-n4">
              En savoir plus <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
            <v-btn color="#2465aa" dark text class="ml-15" href="https://github.com/SammyMERAZGA/GCR" target="_blank">
              Code source <v-icon right class="mb-1">fab fa-github</v-icon>
            </v-btn>
          </div>
        </v-col>
        <v-col cols="12" class="padd topInverse">
          <div class="second">
            <div class="secondchild1" id="contact">
              <v-row>
                <v-col cols="7">
                  <h1 class="white--text mb-5 text-center">
                    Travaillons ensemble sur<br />votre prochain projet !
                  </h1>
                  <p class="grey--text text-center">
                    N'hésitez pas à me contacter pour me donner vos avis sur mon
                    portfolio aussi !<br />
                  </p>
                </v-col>
                <v-col cols="5">
                  <v-btn tile color="#2465aa" class="rounded-xl" dark id="btnContact">
                    Contact
                  </v-btn>
                </v-col>
              </v-row>
            </div>
          </div>
          <v-toolbar class="topTolbar" color="#111111" dark flat>
            <div
              style="
                position: absolute;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
            >
            </div>
          </v-toolbar>
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

#btnContact {
  margin-top: 20%;
  margin-left: 30%;
}
</style>
