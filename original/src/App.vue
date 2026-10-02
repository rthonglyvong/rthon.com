<template>
  <v-app app>
    <v-card class="overflow-hidden">
      <v-app-bar
        app
        absolute
        color="#fcb69f"
        dark
        shrink-on-scroll
        src="../src/assets/bg.jpg"
        scroll-target="#scrolling-techniques-2"
      >
        <template v-slot:img="{ props }">
          <v-img
            v-bind="props"
            gradient="to top right, rgba(19,84,122,.5), rgba(128,208,199,.8)"
          ></v-img>
        </template>
        <v-spacer></v-spacer>

<v-btn icon>
          <a href="https://www.linkedin.com/in/%F0%9F%8D%B5-ricky-thonglyvong-36330858/">
            <v-icon>mdi-linkedin</v-icon>
          </a>
        </v-btn>
        <v-btn icon>
          <a href="https://github.com/rthonglyvong">
            <v-icon>mdi-github</v-icon>
          </a>
        </v-btn>

        <v-btn icon>
          <a href="mailto:ricky@rthon.com">
            <v-icon>mdi-email</v-icon>
          </a>
        </v-btn>
      </v-app-bar>
        <v-content class="background">
          <v-container fluid pa-0 no-gutters>
            <v-row no-gutters>
              <v-spacer />
              <v-col lg="8" md="12" sm="12" xs="12">
                <v-row class="h5em"/>
                <v-row
                  no-gutters
                  class="text-center top-row flex-grow-1 flex-shrink-1"
                >
                  <v-col cols="12" justify="center" align="center">
                    <v-img
                      max-width="200px"
                      src="../src/assets/logo.png"
                    ></v-img>
                  </v-col>
                  <v-col class="mb-4">
                    <h1 class="display-2 font-weight-bold mb-3">
                      Hi, I'm Ricky <br />
                      Thonglyvong
                    </h1>

                    <v-row>
                      <v-col>
                        <p>He/Him</p>
                        <p>I like pastel colors</p>
                        <p>Learning how to draw</p>
                        <p>Learning how to snowboard</p>
                      </v-col>
                    </v-row>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col class="mb-5" cols="12">
                    <v-row justify="center">
                      <div class="text-h2">
                        Projects
                      </div>
                    </v-row>
                    <v-row>
                      <v-spacer />
                      <v-col lg=4 md=4 sm=12 xs=12>
                        <v-card class="mx-auto my-12" max-width="374">
                          <v-img
                            height="250"
                            src="../src/assets/conartist.png"
                          ></v-img>

                          <v-card-title
                            >asynchronous multiplayer websocket drawing game
                            prototype</v-card-title
                          >

                          <v-card-text>
                            <div class="my-4 subtitle-1">
                              VueJS, Spring Boot, WebSockets
                            </div>

                            <div>
                              Inspired by skribbl.io and among us. TODO: hire a
                              designer/artist to create assets and animations...
                              maybe =)
                            </div>
                          </v-card-text>
                          <v-divider class="mx-4"></v-divider>
                          <v-card-actions>
                            <v-btn
                              color="deep-purple lighten-2"
                              text
                              href="http://rthonglyvong.moe"
                            >
                              Demo
                            </v-btn>
                          </v-card-actions>
                        </v-card>
                      </v-col>
                      <v-spacer />
                      <v-col lg=4 md=4 sm=12 xs=12>
                        <v-card class="mx-auto my-12" max-width="374">
                          <v-img
                            height="250"
                            src="../src/assets/vvaifu.png"
                          ></v-img>

                          <v-card-title>shareable quiz</v-card-title>

                          <v-card-text>
                            <div class="my-4 subtitle-1">
                              NextJS, React, AWS Lambda, S3
                            </div>

                            <div>
                              Fun little quiz created by consuming MediaWiki API
                              to generated results. Result previews are
                              generated using an aws lambda to created a
                              screenshot of your results and stored in s3 to be
                              shared through linked previews.
                            </div>
                          </v-card-text>
                          <v-divider class="mx-4"></v-divider>
                          <v-card-actions>
                            <v-btn
                              color="deep-purple lighten-2"
                              text
                              href="https://www.vvaifu.moe"
                            >
                              Demo
                            </v-btn>
                          </v-card-actions>
                        </v-card>
                      </v-col>
                      <v-spacer />
                    </v-row>
                  </v-col>
                </v-row>
              </v-col>
              <v-spacer />
            </v-row>
          </v-container>
        </v-content>
    </v-card>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    //
  }),
};
</script>
<style scoped>
.background {
  background: rgb(238, 236, 236);
  color: #685353;
}
.fill-parent-height {
  height: 100%;
}

.black {
  color: black !important;
}

.v-card__text, .v-card__title {
  word-break: normal !important;
}

a {
  color: white !important;
}

.h5em{
  height: 5em;
}
</style>
