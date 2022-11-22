<template>
  <q-layout view="hHh lpR fff">

    <q-header header elevated class="header" height-hint="98">
      <q-toolbar>
        <q-toolbar-title>

          <q-tabs class="q-ml-xl text-black qtabs" align="left">
            <q-route-tab to="/" label="Startseite"/>
            <q-route-tab to="/impressum" label="Impressum"/>
          </q-tabs>

        </q-toolbar-title>
      </q-toolbar>

    </q-header>

    <div class="box">

      <!-- particles.js -->
      <div id="particles-js">
        <Particles
          id="tsparticles"
          :particlesInit="particlesInit"
          :particlesLoaded="particlesLoaded"
          :options="{
                    fullScreen: {
                        enable: false,
                        zIndex: 0,
                      },
                    background: {
                        color: {
                            value: 'transparent'
                        }
                    },
                    fpsLimit: 120,
                    interactivity: {
                        events: {
                            onClick: {
                                enable: false,
                                mode: 'push'
                            },
                            onHover: {
                                enable: true,
                                mode: 'repulse'
                            },
                            resize: true
                        },
                        modes: {
                            bubble: {
                                distance: 400,
                                duration: 2,
                                opacity: 0.8,
                                size: 40
                            },
                            push: {
                                quantity: 4
                            },
                            repulse: {
                                distance: 100,
                                duration: 0.4
                            }
                        }
                    },
                    particles: {
                        color: {
                            value: '#000000'
                        },
                        links: {
                            color: 'rgba(255,255,255,0.25)',
                            distance: 150,
                            enable: true,
                            opacity: 0.1,
                            width: 1
                        },
                        collisions: {
                            enable: false
                        },
                        move: {
                            direction: 'none',
                            enable: true,
                            outMode: 'bounce',
                            random: false,
                            speed: 1,
                            straight: false
                        },
                        number: {
                            density: {
                                enable: true,
                                area: 800
                            },
                            value: 80
                        },
                        opacity: {
                            value: 0.2
                        },
                        shape: {
                            type: 'circle'
                        },
                        size: {
                            random: true,
                            value: 5
                        }
                    },
                    detectRetina: true
                }"
        />
      </div>

      <div class="waves"></div>

      <!-- Headertext -->
      <div class="text not-selectable absolute-center q-pb-lg">
        <span class="name fontsize-36">
          Fabio Carta
          <br>
        </span>

        <span class="infotext fontsize-20">
          staatl. gepr. informationstechnischer Assistent
          <br>
        Student der Medieninformatik
        </span>
      </div>

      <!-- SVG Trenner + Wave-->
      <div class="custom-shape-divider-top-1668202345">
        <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
          <path
            d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z"
            opacity=".25" class="shape-fill"></path>
          <path
            d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z"
            opacity=".5" class="shape-fill"></path>
          <path
            d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z"
            class="shape-fill"></path>
        </svg>

        <svg width="0" height="0">
          <linearGradient id="lgrad" x1="0%" y1="50%" x2="100%" y2="50%">
            <stop offset="0%" style="stop-color:rgb(133,42,174);stop-opacity:1.00"/>
            <stop offset="100%" style="stop-color:rgb(60,88,181);stop-opacity:1.00"/>
          </linearGradient>
        </svg>

      </div>
    </div>


    <!-- Footer -->
    <q-footer elevated class="text-white footerLinks">

      <div class="q-pa-md row justify-center footerBtn">

        <q-btn class="q-pa-sm q-ma-sm justify-center"
               icon="ion-mail"
               href="mailto: fcarta@outlook.de">
        </q-btn>

        <q-btn class="q-pa-sm q-ma-sm justify-center "
               icon="ion-logo-github"
               href="https://github.com/FabioCarta/">
        </q-btn>

        <q-btn class="q-pa-sm q-ma-sm justify-center"
               icon="ion-logo-linkedin"
               href="https://www.linkedin.com/in/fabio-carta-618a85219/">
        </q-btn>

        <q-page-scroller position="bottom-right" :scroll-offset="150" :offset="[18, 18]">
          <q-btn fab icon="keyboard_arrow_up" color="accent"/>
        </q-page-scroller>

      </div>

      <q-toolbar>
        <q-toolbar-title>
          <div class="copyright">Copyright (c) Fabio Carta</div>
          <a class="privacy" href="/#/privacy" type="a">Datenschutzerklärung</a>
        </q-toolbar-title>
      </q-toolbar>

    </q-footer>

    <q-page-container>


      <router-view/>
    </q-page-container>

  </q-layout>

</template>



<script setup>
import {loadFull} from "tsparticles";

const particlesInit = async engine => {
  await loadFull(engine);
};

const particlesLoaded = async container => {
  console.log("Particles container loaded", container);
};
</script>



<script>

var doc, bod, htm;
addEventListener("load", function () {
  doc = document;
  bod = doc.body;
  htm = doc.documentElement;
  addEventListener("scroll", function () {
    doc.querySelector("header").style.opacity =
      htm.scrollTop > 500 ? "0.9" : "0";
  });
});

export default {
  name: 'MainLayout',
}

</script>



<style>
.copyright {
  font-size: 12px;
}

.privacy {
  color: #CDDEEE;
  font-size: 12px;
}

.header {
  background-color: white;
  opacity: 0;
}

.footerBtn {
  background-color: #314150;
}

.footerLinks {
  background-color: #293744;
}

.waves {
  width: 100%;
  height: 40vh;
  background-image: linear-gradient(90deg, #852aae, #3c58b5);
}

.box {
  width: 100%;
  height: calc(40vh + 25px);
  position: relative;
  text-align: center;
  color: white;
  z-index: 1;
}


#tsparticles {
  width: 100%;
  height: 40vh;
  position: relative;
  text-align: center;
  color: white;
}


.custom-shape-divider-top-1668202345 svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 25px;
}

.custom-shape-divider-top-1668202345 .shape-fill {
  fill: url(#lgrad);
}

#particles-js {
  position: absolute;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: transparent;
  background-repeat: no-repeat;
  background-size: contain;
  left: 0;
  z-index: 0;
}

.not-selectable {
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.name {
  font-family: 'Raleway';
  font-weight: 200;
  /*font-size: 5vw;*/
  opacity: 1;
  border-bottom: 1px solid;
  text-decoration-thickness: 2px;
  color: #b176ff;
}

.infotext {
  font-family: 'Raleway';
  font-weight: 200;
  font-size: 2vw;
  opacity: 1;
  color: #b176ff;
}

@media only screen and (max-device-width: 480px) {
  .qtabs{
    margin-left: 0;
  }
}

.fontsize-8 {
  font-size: calc(8px + (18 - 8) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-9 {
  font-size: calc(9px + (20 - 9) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-10 {
  font-size: calc(10px + (22 - 10) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-11 {
  font-size: calc(11px + (24 - 11) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-12 {
  font-size: calc(12px + (26 - 12) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-13 {
  font-size: calc(13px + (28 - 13) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-14 {
  font-size: calc(14px + (30 - 14) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-15 {
  font-size: calc(15px + (32 - 15) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-16 {
  font-size: calc(16px + (34 - 16) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-17 {
  font-size: calc(17px + (36 - 17) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-18 {
  font-size: calc(18px + (38 - 18) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-19 {
  font-size: calc(19px + (40 - 19) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-20 {
  font-size: calc(20px + (42 - 20) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-21 {
  font-size: calc(21px + (44 - 21) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-22 {
  font-size: calc(22px + (46 - 22) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-23 {
  font-size: calc(23px + (48 - 23) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-24 {
  font-size: calc(24px + (50 - 24) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-25 {
  font-size: calc(25px + (52 - 25) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-26 {
  font-size: calc(26px + (54 - 26) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-27 {
  font-size: calc(27px + (56 - 27) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-28 {
  font-size: calc(28px + (58 - 28) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-29 {
  font-size: calc(29px + (60 - 29) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-30 {
  font-size: calc(30px + (62 - 30) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-31 {
  font-size: calc(31px + (64 - 31) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-32 {
  font-size: calc(32px + (66 - 32) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-33 {
  font-size: calc(33px + (68 - 33) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-34 {
  font-size: calc(34px + (70 - 34) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-35 {
  font-size: calc(35px + (72 - 35) * ((100vw - 300px) / (1800 - 300))) !important;
}

.fontsize-36 {
  font-size: calc(36px + (74 - 36) * ((100vw - 300px) / (1800 - 300))) !important;
}


</style>
