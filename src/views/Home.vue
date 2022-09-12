<template>
  <v-layout column justify-center align-center class="mt-4 pt-2">
    <VueCompareImage
      class="hidden-md-and-down"
      hover
      :style="{ minWidth: '1300px' }"
      :sliderLineWidth="sliderLine"
      :handleSize="hSize"
      :leftImage="leftImage"
      :rightImage="rightImage"
      :sliderPositionPercentage="sliderPosition"
    />
    <VueCompareImage
      class="hidden-lg-and-up"
      hover
      :style="{ maxWidth: '400px' }"
      :sliderLineWidth="sliderLine"
      :handleSize="hSize"
      :leftImage="leftImage2"
      :rightImage="rightImage2"
      :sliderPositionPercentage="sliderPosition"
    />

    <br>

    <vue-typer class="headline" :repeat="0" text="Cian Larkin"></vue-typer>
    <vue-typer
      :text="text1"
      :repeat="Infinity"
      :shuffle="false"
      initial-action="erasing"
      :pre-type-delay="70"
      :type-delay="70"
      :pre-erase-delay="1980"
      :erase-delay="150"
      erase-style="select-back"
      :erase-on-complete="false"
      caret-animation="smooth"
    ></vue-typer>
    <br>
    <v-flex xs12 sm6 md4 lg4 xl4>
      <v-card flat color="transparent" max-width="500">
        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">
              <span>About</span>
              <span class="blue--text">Me</span>
            </h3>
            <div>
              <p>
                Hello! I’m Cian Larkin. I'm a Computer science student who loves 
                <span
                  class="blue--text font-weight-bold"
                >PROGRAMMING </span>& developing projects which I have done over the course of my degree. 
A diligent and positive person with excellent communication skills developed over years of experience in the hospitality industry. Works well within a team having collaborated on various group projects. I'm always hungry for new transferable skills and 
 take pride in being a fast learner. <br><br>When I'm not focused on my education and personal projects I'm usually playing the guitar or ruthlessly competing against friends in any given sport :)
              </p>
            </div>
          </div>
        </v-card-title>

        <v-card-actions class="hidden-sm-and-down">
          <v-btn
            v-for="icon in icons"
            :key="icon.icon"
            fab
            dark
            outline
            color="blue"
            :href="icon.href"
            target="_blank"
          >
            <v-icon dark>{{icon.icon}}</v-icon>
          </v-btn>
        </v-card-actions>

        <v-card-actions class="hidden-md-and-up justify-center">
          <v-btn
            v-for="icon in icons"
            :key="icon.icon"
            small
            fab
            dark
            outline
            color="blue"
            :href="icon.href"
            target="_blank"
          >
            <v-icon dark>{{icon.icon}}</v-icon>
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import { VueTyper } from "vue-typer";
import VueCompareImage from "vue-compare-image";

export default {
  metaInfo: {
    title: "Home",
    titleTemplate: "%s ← Cian Larkin",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      { name: "description", content: "Cian Larkin's Portfolio" },
      { charset: "utf-8" },
      { property: "og:title", content: "Cian's Space" },
      { property: "og:site_name", content: "Cian's Space" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "" },
      {
        property: "og:image",
        content: "https://i.imgur.com/Dcz2PGx.jpg"
      },
      { property: "og:description", content: "Cian Larkin's Portfolio" }
    ]
  },
  components: {
    "vue-typer": VueTyper,
    VueCompareImage
  },
  data() {
    return {
      icons: [
        { href: "https://github.com/C-Larkin02", icon: "fab fa-github" },
        // {
        //   href: "",
        //   icon: "fab fa-stack-overflow"
        // },
        // { href: "", icon: "fab fa-twitter" },
        {
          href: "https://www.linkedin.com/in/cianlarkin02/",
          icon: "fab fa-linkedin-in"
        },
        // {
        //   href: "",
        //   icon: "fab fa-xing"
        // },
        // {
        //   href: "",
        //   icon: "fab fa-facebook-f"
        // },
        // { href: "", icon: "fab fa-instagram" }
      ],
      text1: ["Computer Science Student", "Software Engineer", "Web Developer"],
      leftImage: "https://i.imgur.com/QALxhwO.jpeg",
      rightImage: "https://i.imgur.com/FaVdl7E.jpeg",
      leftImage2: "https://i.imgur.com/QALxhwO.jpeg",
      rightImage2: "https://i.imgur.com/FaVdl7E.jpeg",
      sliderLine: 0,
      hSize: 0,
      sliderPosition: 0.5
    };
  }
};
</script>
<style>
@keyframes rocking {
  0%,
  100% {
    transform: rotateZ(-10deg);
  }

  50% {
    transform: rotateZ(10deg);
  }
}

.vue-typer {
  font-family: Arial, "Helvetica Neue", Helvetica, sans-serif;
}
.vue-typer .custom.char.typed {
  color: rgb(20, 103, 212);
}
.vue-typer .custom.char.selected {
  color: #000000;
}

.vue-typer .custom.caret {
  animation: rocking 1s ease-in-out 0s infinite;
}
.vue-typer .custom.caret.typing {
  background-color: rgb(16, 108, 199);
}
.vue-typer .custom.caret.selecting {
  display: inline-block;
  background-color: #e91e63;
}
</style>

