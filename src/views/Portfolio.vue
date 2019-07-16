<template>
  <div class="wrapper">
    <parallax class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout">
          <div
            class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100"
          >
            <h1 class="title titulo">My Portfolio Page</h1>
            <h4>
              The websites below are the projects that I have completed or am currently working on to express my skills in programming. Take a look...
            </h4>
            <br />
            <md-button
              href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
              class="md-success md-lg"
              target="_blank"
              ><i class="fas fa-play"></i> Watch video</md-button
            >
          </div>
        </div>
      </div>
    </parallax>

  <div class="main main-raised section">
  <div class="websites">

    <md-card class="fundo">
      
        <md-card-media md-ratio="1:1">
          <img src="https://images.pexels.com/photos/808465/pexels-photo-808465.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260">
        </md-card-media>

        <div class="md-layout">
                  <div class="md-layout-item md-size-3">
                    <md-button class="md-success">A Mountain Adventure</md-button>
                  </div>
                </div>
    </md-card>

    <md-card>
        <md-card-media md-ratio="1:1">
          <img src="https://images.pexels.com/photos/1598505/pexels-photo-1598505.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260" alt="Skyscraper" class="sneaker">
        </md-card-media>

        <div class="md-layout">
                  <div class="md-layout-item md-size-3">
                    <md-button class="md-success">Sneaker Land</md-button>
                  </div>
                </div>
    </md-card>

    <md-card>
        <md-card-media md-ratio="1:1">
          <img src="https://images.pexels.com/photos/216657/pexels-photo-216657.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260" alt="Skyscraper" class="leaf">
        </md-card-media>

        <div class="md-layout">
                  <div class="md-layout-item md-size-3">
                    <md-button class="md-success">UnEarth</md-button>
                  </div>
                </div>
    </md-card>

  </div>

      <div class="section section-contacts">
        <div class="container">
          <div class="md-layout">
            <div class="md-layout-item md-size-66 md-xsmall-size-100 mx-auto">
              <h2 class="text-center title">Work with me</h2>
              <h4 class="text-center description">
                If you're interested in working with me,
                write a few lines about your message and contact me about any further collaboration. I will respond and get back to you in a
                couple of hours.
              </h4>
              <form class="contact-form">
                <div class="md-layout">
                  <div class="md-layout-item md-size-50">
                    <md-field>
                      <label>Your Name</label>
                      <md-input v-model="name" type="text"></md-input>
                    </md-field>
                  </div>
                  <div class="md-layout-item md-size-50">
                    <md-field>
                      <label>Your Email</label>
                      <md-input v-model="email" type="email"></md-input>
                    </md-field>
                  </div>
                </div>
                <md-field maxlength="5">
                  <label>Your Message</label>
                  <md-textarea v-model="message"></md-textarea>
                </md-field>
                <div class="md-layout">
                  <div class="md-layout-item md-size-33 mx-auto text-center">
                    <md-button class="md-success">Send Message</md-button>
                  </div>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>

export default {
   name: 'MediaCover',
  bodyClass: "landing-page",
  props: {
    header: {
      type: String,
      default: require("@/assets/img/bg7.jpg")
    },
    teamImg1: {
      type: String,
      default: require("@/assets/img/faces/avatar.jpg")
    },
    teamImg2: {
      type: String,
      default: require("@/assets/img/faces/christian.jpg")
    },
    teamImg3: {
      type: String,
      default: require("@/assets/img/faces/kendall.jpg")
    }
  },
  data() {
    return {
      name: null,
      email: null,
      message: null
    };
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`
      };
    }
  }
};
</script>

<style lang="scss" scoped>

.leaf{
  height: 219px;
}

.sneaker{
  height: 219px;
}

.websites{
  text-align: center;
}
.titulo{
  text-align: left;
}

.md-card-actions.text-center {
  display: flex;
  justify-content: center !important;
}
.contact-form {
  margin-top: 30px;
}

.md-has-textarea + .md-layout {
  margin-top: 15px;
}

.md-card {
    width: 320px;
    margin: 4px;
    display: inline-block;
    vertical-align: top;
    background-color: white !important;
    box-shadow: 0px 0px 25px 0px !important;
  }

.md-card-header{
  background-color: transparent !important;
  box-shadow: none !important;
}

.md-layout{
  margin-bottom: 15%;
}

.section{
  padding-top: 70px;
  padding-bottom: 0px;
}
</style>