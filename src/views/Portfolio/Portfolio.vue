<template>
  <v-container grid-list-xl>
    <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <v-flex v-for="portfolio in portfolios" :key="portfolio.src" xs12 sm12 md4 lg4 xl4>
        <v-card
          :to="'/portfolio/'+(portfolio.title).toLowerCase()"
          hover
          flat
          color="transparent"
          height="230"
        >
          <v-card-title></v-card-title>
          <v-img :src="portfolio.src" aspect-ratio="2.75" height="130" contain></v-img>
          <v-card-title primary-title class="justify-center">
            <v-flex text-xs-center subheading font-weight-bold>{{portfolio.title}}</v-flex>
          </v-card-title>
        </v-card>
      </v-flex>
    </v-layout>
    <v-footer color=rgb(250,250,250)>
    <v-col
      class="text-center justify-center"
      cols="12"
    >
      <strong>Hi! I'm currently working on this section of my website. It's not finished yet. Please come back soon to see what I've been working on :)</strong>
    </v-col>
  </v-footer>
  </v-container>
  
</template>

<script>
export default {
  metaInfo: {
    title: "Portfolio",
    titleTemplate: "%s ← Cian's Space",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      {
        name: "description",
        content:
          "Cian Larkin's Portfolio Web Development Video Editing Graphic Design Front-End Advetising"
      },
      { charset: "utf-8" },
      { property: "og:title", content: "Cian' Space" },
      { property: "og:site_name", content: "Cian' Space" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "https://Cian.space" },
      {
        property: "og:image",
        content: "https://i.imgur.com/Dcz2PGx.jpg"
      },
      {
        property: "og:description",
        content:
          "Cian Larkin's Portfolio Web Development Video Editing Graphic Design Front-End Advetising"
      }
    ]
  },
  data() {
    return {
      portfolios: [
        {
          src: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQBrj1oQ9gUmigKFE2eBTa-lhApnQLhnKbgmg&usqp=CAU",
          title: "Personal Projects"
        },

        {
          src: "data:image/png;base64,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",
          title: "University Projects"
          
        },
        
        // {
        //   src: "https://i.imgur.com/g74mGuU.png",
        //   title: "Graphic"
        // }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
</style>