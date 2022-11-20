<template>






  <q-page-container style="padding-top: 50px">
    <q-page>

  <div class="q-mx-lg row items-start justify-center flex items-stretch">


    <q-card flat class="flex-item">

      <q-card-section class="vertical-top text-center q-mt-sm">
        <q-avatar color="accent" text-color="white" icon="person" />
        <!--          <q-icon name="computer" size="3rem"/>-->

      </q-card-section>

      <q-card-section>
        <div class="text-h6 text-center">Persönliches</div>
        <div class="text-subtitle2 text-center">
          <br>Name:<br>
          Fabio Carta<br><br>
          Alter:<br>
          28<br><br>
          Wohnort: <br>Köln<br><br>
          Hobbys:<br>
          Musikproduktion<br>DJing<br>Gaming
        </div>
      </q-card-section>
    </q-card>

    <q-card flat class="flex-item">

  <q-card-section class="vertical-top text-center q-mt-sm">

    <q-avatar color="accent" text-color="white" icon="code" />
<!--         <q-icon name="code" size="3rem"/>-->


  </q-card-section>

  <q-card-section>

  <div class="text-h6 text-center">Sprachen</div>
  <div class="text-subtitle2 text-center">
    <br>
    C
    <br>
    C#
    <br>

    Java
    <br>
    Kotlin
    <br>
    Prolog
    <br>Scala<br>
    <br>
    SQL
    <br>
    PHP
    <br><br>
    XML
    <br>
    <br>
    HTML
    <br>
    CSS
    <br>
    JavaScript
</div>
  </q-card-section>
    </q-card>

    <q-card flat class="flex-item">

      <q-card-section class="vertical-top text-center q-mt-sm">
        <q-avatar color="accent" text-color="white" icon="computer" />
<!--          <q-icon name="computer" size="3rem"/>-->
      </q-card-section>

      <q-card-section>
        <div class="text-h6 text-center">Software & Tools</div>
        <div class="text-subtitle2 text-center">
          <br>
          IntelliJ, CLion, Webstorm, <br> Visual Studio Code, Android Studio<br><br>

          Git, Github<br><br>

          Node.js<br>
          Quasar<br>
          AWS, Firebase<br>Apache2<br>

          MySQL, OracleDB<br>

          MS Office<br>
          V-Modell XT<br>
          Figma, Sketch<br><br>

          Linux (Ubuntu), Windows 10, Mac OSX<br>
        </div>
      </q-card-section>
    </q-card>


<div class="trenner"></div>


    <q-card flat class="flex-item">

      <q-card-section class="vertical-top text-center q-mt-sm">

        <q-avatar color="accent" text-color="white" icon="school" />
        <!--         <q-icon name="code" size="3rem"/>-->


      </q-card-section>

      <q-card-section>
        <div class="text-h6 text-center">Ausbildung</div>
        <div class="text-subtitle2">
          <br>

          <table class="flex-center table">
            <tr class="tr">
              <td class="td">2013 -<br>bis jetzt </td>
              <td class="td">Medieninformatik B. Sc.<br>Technische Hochschule Köln</td>
            </tr>
            <tr></tr>
            <tr class="tr">
              <td class="td">2010 - 2013</td>
              <td class="td">staatl. gepr. informationstechnischer Assistent<br>Fachhochschulreife<br>Georg-Simon-Ohm-Berufskolleg, Köln</td>
            </tr>
          </table>

</div>
      </q-card-section>
    </q-card>

    <q-card flat class="flex-item">

      <q-card-section class="vertical-top text-center q-mt-sm">
        <q-avatar color="accent" text-color="white" icon="work" />
        <!--          <q-icon name="computer" size="3rem"/>-->
      </q-card-section>

      <q-card-section>
        <div class="text-h6 text-center">Beruflicher Werdegang</div>
        <div class="text-subtitle2">
          <br>

          <table class="flex-center table">
            <tr class="tr">
              <td class="td">2016 -<br>bis jetzt </td>
              <td class="td">Kodierkraft<br>Deutsche Post AG, Köln</td>
            </tr>
            <tr></tr>
            <tr class="tr">
              <td class="td">2015 - 2016</td>
              <td class="td">Warenverräumer<br>Tempus GmbH & Co. KG, Köln</td>
            </tr>
          </table>

        </div>
      </q-card-section>
    </q-card>


    <q-card flat class="flex-item">

      <q-card-section class="vertical-top text-center q-mt-sm">
        <q-avatar color="accent" text-color="white" icon="workspace_premium" />
        <!--          <q-icon name="computer" size="3rem"/>-->
      </q-card-section>

      <q-card-section>
        <div class="text-h6 text-center">Zertifikate</div>
        <div class="text-subtitle2 text-center">
          <br>

          <a href="https://1drv.ms/b/s!AmCdGfvbfPRpjUpzydfdzRh3PfjN?e=gFf3mZ" target="_blank">Object-Oriented Programming with Java, part I</a>
          <br>
          University of Helsinki, MOOC

        </div>
      </q-card-section>
    </q-card>

    </div>

    </q-page>
  </q-page-container>

</template>





<script>
import { defineComponent } from 'vue'


export default defineComponent({
  name: 'IndexPage'
})

</script>





<style>

.flex-item{
  width: 33%;
}

.td{
  padding: 20px;
}

.table{
  margin-left: auto;
  margin-right: auto;
}

.trenner{
  width:100%;
  height:80px;
  background-color:transparent;
}
</style>
