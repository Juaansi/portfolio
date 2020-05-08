<template>
  <v-app id="app">
      <v-toolbar 
      dense
      flat
      min-width="100vw"
      absolute="true"
      color="rgba(255, 255, 255, 0)"
      >
       <!-- <v-app-bar-nav-icon>
          
        </v-app-bar-nav-icon>
        -->
        <v-spacer></v-spacer>
        <a href="https://www.instagram.com/juaansi/" target="blank">
          <v-btn icon>
            <v-icon>mdi-instagram</v-icon>
          </v-btn>
        </a>
      </v-toolbar>
      <v-row>
        <v-row>
          <!-- Landing image -->
          <v-img
            src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977267863-JHGSFYLENEEPTXC4RT90/ke17ZwdGBToddI8pDm48kCX-V5vw-8h9IBXN10-_8XN7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0p4Wyba38KfG317vYluk45_zZdtnDCZTLKcP2mivxmYi50xvY5saIGKMgOza9mH4XA/DSC01054.jpg?format=2500w"
            aspect-ratio="1"
            class="grey lighten-2"
            fluid
            height="100vh"
            >
            <h1 id="landingPageTitle">
              Johannes Olsen Portfolio
            </h1>
            <template v-slot:placeholder>
              <v-row
                class="fill-height ma-0"
                align="center"
                justify="center"
                >
                <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
              </v-row>
            </template>
          </v-img>
        </v-row>
      </v-row>
      <!-- These are the pictures -->
      <v-row id="picture_grid" no-gutters>
        <v-col cols>
          <!-- The deers -->
          <v-img
          src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977289893-1HQNPN96NWNN57Y3V0RQ/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/IMG_5683.jpg?format=2500w"
          aspect-ratio="1"    
          @click.stop="dialogDeers = !dialogDeer"
          >
          </v-img>
          <v-dialog 
            v-model="dialogDeers"
            dark
            width="min-content"
            >
              <v-card>
                <v-card-title class="headline" @click="dialogDeers = !dialogDeers">
                <v-img
                  src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977289893-1HQNPN96NWNN57Y3V0RQ/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/IMG_5683.jpg?format=2500w"
                  max-height="70vh"
                  contain
                  >
                </v-img>
                </v-card-title>
                  <v-card-actions>
                  <v-card-text> This was for an UX/CC research walk. These aren't dolphins
                    </v-card-text>
                      </v-card-actions>
                </v-card>
            </v-dialog>
        </v-col>
        <v-col>
           <v-row no-gutters>
              <v-col cols>
                <!-- Esbjerg harbor -->
                  <v-img
                  src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977315477-ADEH0JOTFZ5ZIKK220DF/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/IMG_5918.jpg?format=2500w"
                  aspect-ratio="2"    
                  @click.stop="dialogHarbor = !dialogHarbor"
                  >
                </v-img>
                <v-dialog 
                  v-model="dialogHarbor"
                  dark
                  width="min-content"
                  >
                  <v-card>
                    <v-card-title class="headline" @click="dialogHarbor = !dialogHarbor">
                      <v-img
                  src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977315477-ADEH0JOTFZ5ZIKK220DF/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/IMG_5918.jpg?format=2500w"
                        max-height="70vh"
                      contain
                      >
                      </v-img>
                      </v-card-title>
                      <v-card-actions>
                          <v-card-text> This was taken on the way to Fanø for AV Production for CMS
                          </v-card-text>
                        </v-card-actions>
                    </v-card>
                </v-dialog>
              </v-col>
           </v-row>
           <v-row no-gutters>
              <v-col> 
                <!-- Daniel -->
                <v-img
                  src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977308696-KBOUA0VCXVDWLZ53KXHP/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/IMG_5782-2.jpg?format=2500w"
                  aspect-ratio="1"    
                  @click.stop="dialogDaniel = !dialogDaniel"
                  >
                </v-img>
                <v-dialog 
                  v-model="dialogDaniel"
                  dark
                  width="min-content"
                  >
                  <v-card>
                    <v-card-title class="headline" @click="dialogDaniel = !dialogDaniel">
                      <v-img
                        src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977308696-KBOUA0VCXVDWLZ53KXHP/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/IMG_5782-2.jpg?format=2500w"
                        max-height="70vh"
                      contain
                      >
                      </v-img>
                      </v-card-title>
                      <v-card-actions>
                          <v-card-text> Daniel Radosa looking serious for his upcoming music album
                          </v-card-text>
                        </v-card-actions>
                    </v-card>
                </v-dialog>
              </v-col>
              <v-col> 
                <!-- Raul -->
                <v-img
                  src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977300517-L10M718BSW0DJPPGW2RI/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/IMG_5719-2.jpg?format=2500w"
                  aspect-ratio="1"    
                  @click.stop="dialogRaul = !dialogRaul"
                  >
                </v-img>
                <v-dialog 
                  v-model="dialogRaul"
                  dark
                  width="min-content"
                  >
                  <v-card>
                    <v-card-title class="headline" @click="dialogRaul = !dialogRaul">
                      <v-img
                        src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1587977300517-L10M718BSW0DJPPGW2RI/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/IMG_5719-2.jpg?format=2500w"
                        max-height="70vh"
                      contain
                      >
                      </v-img>
                      </v-card-title>
                      <v-card-actions>
                          <v-card-text> Big daddy Raul posing for his movie poster, looking like a real hunk
                          </v-card-text>
                        </v-card-actions>
                    </v-card>
                </v-dialog>
              </v-col>
           </v-row>
        </v-col>
      </v-row>
        <v-row no-gutters>
        <!-- Video CV -->
          <v-col id="videoCV"> 
              <iframe width="100%" height="450px" src="https://www.youtube.com/embed/gx75ygoavUQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </v-col>
          <v-col>
            <h3 id="videoTitle">
              Video CV
            </h3>
            <p id="videoDescription">
              This is a 2 minute video CV. 
              <br>
              If you want to get to know in me in a fraction of the time.
              <br>
              You can see where come from, get the know the background, what my skils are, and what kind of employee you can expect form me.
            </p>
          </v-col>
        </v-row>
        <!-- Commercial video -->
        <v-row no-gutters>
          <v-col id="commercialVideo">
            <iframe width="100%" height="450px" src="https://www.youtube.com/embed/5e5RCkD0YLM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </v-col>
          <v-col>
            <h3 id="videoTitle">
              Commercial project
            </h3>
            <p id="videoDescription">
              This is a group project. The idea is that throughout the day, we often forget to drink.
              <br> 
              The project has to be at maximum 20 seconds. That mean that we have to somehow convey a product, a message, in a meaningful way that is easy to understand. 
              <br>
              In 20 seconds, my team and I managed to squeeze an entire day what goes on in the world of this man.
              See that he is active, keeps his focus in the workplace, has a date at night, and goes to bed tired. 
              <br>
              <br>
              Filmmaker and editor: Johannes Olsen
              <br>
              Actor/actress: Raul Albu-Octavia & Suong Vo

            </p>
          </v-col>
        </v-row>
      <v-row>
        <!-- About me section -->

        <v-img id="aboutMeImage"
          src="https://images.squarespace-cdn.com/content/v1/54e33094e4b0cb82a5b2556b/1588935044789-JZZIGEX87RWAFHKC23BZ/ke17ZwdGBToddI8pDm48kNvT88LknE-K9M4pGNO0Iqd7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z5QPOohDIaIeljMHgDF5CVlOqpeNLcJ80NK65_fV7S1UbeDbaZv1s3QfpIA4TYnL5Qao8BosUKjCVjCf8TKewJIH3bqxw7fF48mhrq5Ulr0Hg/2019+what+happened.00_05_08_21.Still002.png?format=2500w"
          no gutters
          height="80vh"
          >
          <h3 id="aboutMeTitle">About me</h3>
          <h4 id="aboutMeSubtitle">
            Multimediadesigner, Film- and TV-Technician
          </h4>
          <p id="aboutMeText">
            I am a multimediadesigner student, and graduated from Next København in Film and TV industry. 
            <br>
            I have an extensive experience in making short films, editing, news coverage, and as a live event cameraman.
            <br>
            <br>
            You can click on the images to seem them in bigger window
            <br>
            Go to the top of the page and click on my instagram page and give me a follow, you weeb. 
          </p>

        </v-img>
      </v-row>
      <!-- Email section 
      <v-col>
        <h2 center>
          Let me know what you think
        </h2>
        <v-form method="post" action="https://www.getform.org/f/c40acefd-7eb8-4322-b90b-69ac1d66f242" id="nativeForm" v-model="valid">
          <v-text-field
            label="Name"
            v-model="name"
            :rules="nameRules"
            :counter="20"
            required
            name="message"
            >
          </v-text-field>
          <v-text-field
            label="E-mail"
            v-model="email"
            :rules="emailRules"
            required
            name="mail"
            >
          </v-text-field>
          <v-textarea label="Write me a message"></v-textarea>
          <v-btn @click="submit" :disabled="!valid">Send</v-btn>
        </v-form>
      </v-col>
      -->
      
  </v-app>
</template>

<script>


export default {
  name: 'App',
  data() {
    return {
      dialogDeers: false,
      dialogHarbor: false,
      dialogDaniel: false,
      dialogRaul: false,
    }
  }
};



</script>

<!--
<script>
    export default {
      name: 'contact',

      data () {
         return { 
            valid: false,
            name: '',
            nameRules: [
              (v) => !!v || 'Name is required',
              (v) => v.length <= 20 || 'Name must be less than 20 characters'
            ],
            email: '',
            emailRules: [
              (v) => !!v || 'E-mail is required',
              (v) => /^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(v) || 'E-mail must be valid'
            ]
          }
        },
        methods: {
          submit() {
            nativeForm.submit()
          }
        }
      }
  </script>
  -->
<style>
@import url('https://fonts.googleapis.com/css?family=Baloo+2|Comfortaa|Dancing+Script&display=swap');

#videoTitle {
  padding: 25px;
  text-align: center;
  font-family: 'Baloo 2', cursive;
  font-size: 35px;
  outline: darkgrey;
}
#videoDescription {
  padding: 25px;
  font-family: 'Comfortaa', cursive;


}
#headerTitle {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

#landingPageTitle {
  font-size: 55px;
  margin: 50px;
  font-family: 'Dancing Script', cursive;
  text-align: center;
}

#aboutMeTitle {
  font-size: 45px;
  padding: 35px 0px 15px 45px;
  font-family: 'Baloo 2', cursive;
}
h4 {
  padding: 0 0 0 45px;
    font-family: 'Baloo 2', cursive;
}
#aboutMeText {
  contain: content;
  padding: 0 0 0 45px;
  font-size: 15px;
  font-family: 'Comfortaa', cursive;
  text-shadow: white 1px 1px;
}
a {
  text-decoration: none;
}


</style>