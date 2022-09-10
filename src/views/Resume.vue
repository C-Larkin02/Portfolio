<template>
  <v-layout row justify-center align-center wrap class="mt-4 pt-2">
    <v-flex xs12 sm12 md5 lg6 xl6 class="mt-4 pt-4">
      <h2 class="mb-4 pl-4 pt-2">Education</h2>
      <v-card-text class="py-0">
        <v-timeline align-top dense>
          <v-timeline-item color="blue" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">2020 -</div>
                <div class="caption font-weight-bold blue--text">PRESENT</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Computer Science and Information Technology</strong>
                <div class="caption mb-2">National University of Ireland Galway</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>
          
          <v-timeline-item color="blue" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">2014 -</div>
                <div class="caption font-weight-bold blue--text">2020</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Junior Certificate and Leaving Certificate</strong>
                <div class="caption mb-2">Bailieboruogh Community School</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="blue" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">2006 -</div>
                <div class="caption font-weight-bold blue--text">2014</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>St Anne's National school</strong>
                <div class="caption mb-2">Primary Education</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>
        </v-timeline>
      </v-card-text>
    </v-flex>
    <v-flex xs12 sm12 md4 lg6 xl6 class="mt-4 pt-2">
      <h2 class="mb-4 pl-4">Experience</h2>
      <v-card-text class="py-0">
        <v-timeline align-top dense>
          <v-timeline-item color="blue" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">SEP 2022 -</div>
                <div class="caption font-weight-bold blue--text"> Present</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Product Builder </strong>
                <div class="caption mb-2">Medtronic</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="blue" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">JAN 2022 -</div>
                <div class="caption font-weight-bold blue--text">APRIL 2022</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>F&B Attendant</strong>
                <div class="caption mb-2">Farnham Estate Gold and Spa Resort</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="blue" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold blue--text">May 2019 -</div>
                <div class="caption font-weight-bold blue--text">OCT 2019</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>General Opperative</strong>
                <div class="caption mb-2">Manor Farm</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>
        </v-timeline>
      </v-card-text>
    </v-flex>
    <v-layout row justify-left align-let wrap class="mt-4 pt-2">
      <!-- <v-flex xs12 sm12 md4 lg5 xl5 class="mx-2 pt-4">
        <h2>
          <span>Design</span>

          <span class="green--text">Skills</span>
        </h2>
        <br>
        <strong>Photoshop</strong>
        <v-progress-linear v-model="buffer1" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>Adobe XD</strong>
        <v-progress-linear v-model="buffer2" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>Zeplin</strong>
        <v-progress-linear v-model="buffer3" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
      </v-flex> -->
      <v-flex xs12 sm12 md4 lg5 xl5 class="mx-2 pt-4">
        <h2>
          <span>Technical</span>
          <span class="blue--text">Skills</span>
        </h2>
        <br>
        <strong>JavaScript&nbsp;&nbsp;&nbsp;&nbsp;Java&nbsp;&nbsp;&nbsp;&nbsp;HTML &nbsp;&nbsp;&nbsp;&nbsp;CSS &nbsp;&nbsp;&nbsp;&nbsp;C &nbsp;&nbsp;&nbsp;&nbsp;VUE &nbsp;&nbsp;&nbsp;Bootstrap &nbsp;&nbsp;&nbsp;&nbsp;SQL &nbsp;&nbsp;&nbsp;&nbsp;MATLAB&nbsp;&nbsp;&nbsp;&nbsp;R</strong>
        <!-- <v-list>
          <v-list-item>
            JavaScript
          </v-list-item>
        </v-list> -->
        <!-- <strong>VUE/NUXT</strong>
        <v-progress-linear v-model="buffer4" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>HTML/CSS</strong>
        <v-progress-linear v-model="buffer5" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>JavaScript</strong>
        <v-progress-linear v-model="buffer6" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear> -->
      </v-flex>
      <div class="mt-4 pt-2">
        <v-btn
          href="https://docs.google.com/document/d/1WSR42FEgUahJuR_RArW1wz7TfUBlgj13zekRidmQgs4/edit?usp=sharing"
          target="_blank"
          color="blue"
          dark
          large
        >
          Download Resume
          <v-icon right dark>fas fa-file-download</v-icon>
        </v-btn>
      </div>
    </v-layout>
  </v-layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Resume",
    titleTemplate: "%s ← cian's Space",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      {
        name: "description",
        content:
          "Vue NUXT HTML CSS JavaScript Design Adobe XD Photoshop Coding Skills Resume Work Web Developer Front-End"
      },
      { charset: "utf-8" },
      { property: "og:title", content: "Cian' Space" },
      { property: "og:site_name", content: "Cian' Space" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "" },
      {
        property: "og:image",
        content: "https://i.imgur.com/Dcz2PGx.jpg"
      },
      {
        property: "og:description",
        content:
          "Vue NUXT HTML CSS JavaScript Design Adobe XD Photoshop Coding Skills Resume Work Web Developer Front-End"
      }
    ]
  },
  data() {
    return {
      value: 0,
      buffer1: 0,
      buffer2: 0,
      buffer3: 0,
      buffer4: 0,
      buffer5: 0,
      buffer6: 0,
      bufferValue: 100,
      interval: 0
    };
  },
  mounted() {
    this.startBuffer();
  },

  beforeDestroy() {
    clearInterval(this.interval);
  },

  methods: {
    startBuffer() {
      this.interval = setInterval(() => {
        this.buffer1 = 90;
        this.buffer2 = 85;
        this.buffer3 = 80;
        this.buffer4 = 80;
        this.buffer5 = 90;
        this.buffer6 = 70;
      }, 800);
    }
  }
};
</script>
<style >
</style>

