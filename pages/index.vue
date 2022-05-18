<template>
  <v-container ma-0 pa-0>
    <v-row class="center" style="margin-top:50px;">
      <v-col cols="6">
        <v-img src="/avatar.jpg" max-height="400" max-width="400" style="border-radius:500px" />
      </v-col>
      <v-col cols="6">
        <h1 class="name">
          KAJA WIEWIORA
        </h1>
        <h2 class="subtitle">
          Master architecture student and aspiring designer
        </h2>
        <div style="margin-top: 30px;">
          <v-icon>mdi-file-pdf-box</v-icon>
          <a id="download_portfolio" href="/kwiewiora_portfolio.pdf" download>Download portfolio</a>
        </div>
      </v-col>
    </v-row>

    <v-row class="center flex-nowrap" align="stretch">
      <v-card hover class="div-wrapper ma-5">
        <h1 class="hidden-text">
          T?F TU DELFT DESIGN STUDIO
        </h1>
        <v-img src="/2.jpg" class="projects" />
      </v-card>
      <v-card hover class="div-wrapper ma-5">
        <h1 class="hidden-text">
          CASSEL COLISEUM COMPETITION PROJECT
        </h1>
        <v-img src="/3.jpg" class="projects" />
      </v-card>
      <v-card hover class="div-wrapper ma-5">
        <h1 class="hidden-text">
          ASTRONOMICAL RESEARCH FACILITY GRADUATION PROJECT
        </h1>
        <v-img src="/4.jpg" class="projects" />
      </v-card>
      <v-card hover class="div-wrapper ma-5">
        <h1 class="hidden-text">
          SPORTS ARENA WARSAW
        </h1>
        <v-img src="/5.jpg" class="projects" />
      </v-card>
    </v-row>
  </v-container>
</template>

<script>
export default {
  layout: 'simpleview'
}
</script>

<style>

.div-wrapper {
  position: relative;
  width:27%;
  display: flex;
  flex-direction: column;
}

.div-wrapper:hover :not(.hidden-text) {
  opacity: 0.7;
}

.div-wrapper:hover .hidden-text {
  opacity:1;
}

.hidden-text {
  font-size: 20px;
  color: black;
  font-family: 'Avenir';
  font-weight: 100;
  text-align: center;
  justify-content: center;
  word-break: normal;
  opacity: 0;
  position: relative;
  top: 100px;
  margin: 0px 20px -20px 20px;
}

.center {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  margin-bottom:100px;
}

.center-screen {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  min-height: 100vh;
}

.avatar {
  margin: auto;
  width: 50%;
  border-radius: 100px;
}

.name {
  font-size: 50px;
  color: #686868;
  font-family: 'Avenir';
  font-weight: 100;
  text-align: center;
}

.subtitle {
  font-size: 25px;
  color: #686868;
  font-family: 'Avenir';
  font-weight: 100;
  text-align: center;
}

.btn {
  width: 130px;
  border-width: 2px;
}

#linkedIn {
  border-color: #0072b1;
  color: #0072b1;
}

#linkedIn:hover {
  background-color: #0072b1;
  color: white;
}

#github {
  border-color: #c9510c;
  color: #c9510c;
}

#github:hover {
  background-color: #c9510c;
  color: white;
}

.links {
  color: rgb(105, 105, 141)  !important;
}

.projects {
  object-fit: contain;
}

#download_portfolio {
  color: black;
}

</style>
