<template>
  <header>
    <h1>Projects</h1>
  </header>
  <Project :projects="projects" />
</template>

<script>
import Project from './Project.vue'
export default {
  components: {
    Project
  },
  data() {
    return {
      projects: [ 
        {
          title: "Datoms",
          link: "https://datoms.io/",
          role: "",
          tags: ["Internship"],
          filename: "Datoms.png",
          stack: ["vue.png", "nodejs.png", "materialize-logo.png", "javascript.png", "chart-js.png", "MongoDB.png"],
          description: "Inverter Dashboard to monitor the inverter status, which include parameters like distilled water level, battery percentage, input-output current and voltage, fuse status, etc"
        },
        {
          title: "Weather Dashboard",
          link: "https://datoms-weather.netlify.app/",
          role: "",
          tags: ["internship", "project"],
          filename: "Datoms-Weather.png",
          stack: ["nodejs.png", "vue.png", "materialize-logo.png"],
          description: "Weather dashboard to check the temperature forecast for the coming week. <Br /> Also to display the current weather condition."
        },
      ]
    }
  }
}
</script>

<style>
header {
  margin: 30px auto;
  border-bottom: 1px solid #bbc7c7;
  max-width: 1200px;
}

@media only screen and (max-width: 1400px) {
  header {
    width: 94%
  }
}

@media only screen and (max-width: 992px) {
  header {
    margin: 20px auto;
    width: 90%;
  }
  header h1 {
    font-size: 24px;
  }
}

@media only screen and (max-width: 768px){
  header {
    width: 90%;
    margin: 10px auto;
  }
}

@media only screen and (max-width: 576px) {
  header {
    width: 95%;
  }
}
</style>