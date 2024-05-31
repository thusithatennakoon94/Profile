<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
              <h1 class="text-grey">Hello,</h1>
              <h1 class="text-white">I'M Thusitha Tennakoon</h1>
              <span class="text-grey">MSc In IT Security (NTU - UK )/ Pgdip In Cyber Security (SLIIT -SL) / BSc in Computer Security (Plymouth-UK) / IBM Cyber Security Analsyt (IBM) </span><br />

              
            </div>
          </v-col>
          <v-col cols="2">
            <div
              style="
                position: absolute;
                z-index: 9999;
                bottom: 0;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
              class="mt-16"
            >
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col cols="5">
            <div style="position: relative; z-index: 9999" class="mt-16">
              <v-img src="i1.png" contain max-height="300"></v-img>
            </div>
          </v-col>
        </v-row>
      </div>
      <v-col cols="12" class="mt-16" id="about">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="egg">
                <v-img src="i2.png" max-height="300" class=""></v-img>
              </div>
            </v-col>
            <v-col cols="12" sm="6">
              <h5 class="mt-16">About Me</h5>
              <div style="width: 120px">
                <v-slider
                  v-model="slider2"
                  color="yellow"
                  label="track-color"
                ></v-slider>
              </div>
              <h4 class="mt-n4" >I am a creative web designer and cybersecurity analyst, adept at crafting visually stunning and secure online experiences</h4>
              <h4 class=""></h4>
              <p class="Black">
                I am a cybersecurity specialist with a strong aptitude for safeguarding digital assets. Holding a Master’s degree in IT Security, I possess extensive hands-on experience in security implementation and incident management. In addition to my expertise in cybersecurity, I am proficient in <b> Vue.js and web development </b>. Driven by curiosity and a commitment to excellence, I am dedicated to making a significant impact in the tech industry.
              </p>

            </v-col>
          </v-row>
        </div>
      </v-col>
      <div class="text-center mt-4"  style="max-width: 100%;">

        <h2>My Skills</h2>
        <div style="width: 100%; max-width: 120px; margin: 0 auto">
          <v-slider
            v-model="slider2"
            color="yellow"
            label="track-color"
          ></v-slider>
        </div>
      </div>
      
      
      <v-col cols="12" sm="12">
        <div class="d-flex justify-center mb-6" style="position: relative; width: 100%;">
         
        </div>
      </v-col>
      <v-col cols="12" id="page">
        <div class="pre">
          <v-row>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="i10.jpg" height="200px" cover></v-img>

                

                <v-card-subtitle>
                  Web Desining / Vue Js / PHP
                </v-card-subtitle>
                <v-card-text >
Scripting, Web App Security, Secure Dev Practices, PHP, C++, SQL, Vue.js
Analytical 
Web Development: PHP, HTML, CSS, JavaScript, Web Frameworks
Python / Java
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="i11.jpg" height="200px" cover></v-img>

             

                <v-card-subtitle>
                  Cyber Security
                </v-card-subtitle>
                <v-card-text>
                  Vulnerability Management, Compliance (ISO 27001, NIST), Security Policies
Incident Response and Recovery: Detection, Containment, Business Continuity
Security Architecture and Design: Standards (ISO 27001, NIST), Network Security, Identity Management
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mx-auto" max-width="344" height="">
                <v-img src="i12.jpg" height="200px" cover></v-img>

              

                <v-card-subtitle>
                  Digital Forensics
                </v-card-subtitle>
                <v-card-text>
                  Analytical and Problem-Solving Skills: Critical Thinking, Troubleshooting, 
                  Digital Forensics and Investigation: Evidence Collection, Incident Analysis 
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-col>
 
     
      
         <div class="d-flex justify-center mb-6">
            <div class="child " >
              <h1>Contact info.</h1>
              
              <v-btn
                icon="fas fa-phone-alt"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br />
              <span class="text-caption"> 074 2820 4375</span> <br />
              
              <v-btn
                icon="fas fa-envelope"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br />
              <span class="text-caption">sampath_bandara@hotmail.com </span> <br />
              <span class="text-caption">thusithatennakoon777@gmail.com </span> <br />
            </div>
          </div>
     
    </v-container>
    <FooterView />
  </v-app>
</template>

<script>
import { defineComponent } from "vue";
import NavBar from "../components/NavBar.vue";
import FooterView from "../components/FooterView.vue";

// Components
//import HelloWorld from '../components/HelloWorld.vue';

export default defineComponent({
  name: "HomeView",
  setup() {
    return {
      slider2: 50,

      items: [
        {
          img: "i3.jpg",
        },
        {
          img: "i4.jpg",
        },
        {
          img: "i5.jpg",
        },
        {
          img: "i6.jpeg",
        },
        {
          img: "i9.jpg",
        },
        {
          img: "i8.jpg",
        },
      ],
    };
  },
  components: {
    NavBar,
    FooterView
},
});
</script>
<style scoped>
.v-container {
  padding: 16px 0 16px 0;
}

.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  width: 100%;
  color: white;
}
.head:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}
.head:after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg);
}
.egg {
  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 356px;
  height: 300px;
  background-color: #fbdf7e;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
}
.first {
  width: 100%;
  height: 280px;
  text-align: center;
  padding: 2rem 2rem;
}
.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;
}
.imgHover {
  padding: 0 200px;
}
.pre {
  width: 100%;
  height: 380px;
  text-align: center;
  padding: 0 200px;
  background-color: #f5f5f5;
}
.hire {
  width: 100%;
  height: 200px;
  padding: 0 200px;
  background-color: #e9e9e9;
  margin-top: -24px;
}

</style>
