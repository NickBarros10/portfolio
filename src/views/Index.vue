<template>
  <div class="wrapper">
    <parallax class="page-header header-filter" :style="headerStyle">
      <div class="md-layout">
        <div class="md-layout-item">
          <div class="image-wrapper">
            <img :src="leaf3" alt="leaf3" class="leaf3" v-show="leafShow" />
            <img :src="leaf2" alt="leaf2" class="leaf2" v-show="leafShow" />
            <img :src="leaf1" alt="leaf1" class="leaf1" v-show="leafShow" />
            <div class="brand">
              <h1>BroCode</h1>
              <hr>
              <br>
              <h3>Programming and Design</h3>
            </div>
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised">
      <div class="section section-basic">
        <div class="container">
          <div class="title">
            <h2>Who I Am</h2>
          </div>
          
        </div>
      </div>
       
      
      <div>
        <div class="text-center">
          <div class="md-layout">
            <div
              class="md-layout-item md-size-66 md-xsmall-size-100 ml-auto mr-auto text-center"
            >
              <h4>
                I am a young guy learning the nature of coding. Along with this, I am developing a passion for the creation and development of websites. Ultimately, my goal is to satisfy future clients by carrying out their specific instructions with love.
              </h4>
            </div>
          </div>
        </div>
      </div>
      <div class="section">
      <div class="container">
      <div class="col-lg-7">

      <!-- Grid row -->
      <div class="row mb-3">

        <!-- Grid column -->
        <div class="col-1">
          <i class="fas fa-share fa-lg accentColor"></i>
        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-xl-10 col-md-11 col-10">
          <h5 class="font-weight-bold mb-3">Progress</h5>
          <p class="black-text">With about 6 months worth of programming experience and education, I am getting closer and closer to being able to provide you with quality content catered towards your digital needs.</p>
        </div>
        <!-- Grid column -->

      </div>
      <!-- Grid row -->

      <!-- Grid row -->
      <div class="row mb-3">

        <!-- Grid column -->
        <div class="col-1">
          <i class="fas fa-share fa-lg accentColor"></i>
        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-xl-10 col-md-11 col-10">
          <h5 class="font-weight-bold mb-3">Creativity</h5>
          <p class="black-text">Aiming to reboot your business' valued brand? Don't worry, as apart from programming, I am aiming my focus on design as well! Let's renovate your brand to the future.</p>
        </div>
        <!-- Grid column -->

      </div>
      <!-- Grid row -->

      <!--Grid row-->
      <div class="row">

        <!-- Grid column -->
        <div class="col-1">
          <i class="fas fa-share fa-lg accentColor"></i>
        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-xl-10 col-md-11 col-10">
          <h5 class="font-weight-bold mb-3">Mission</h5>
          <p class="black-text mb-0">I am currently developing my skills of running businesses in high school. With that, I've learned fast the value of communication. I strive to please and look forward to showing you what I will have to offer!</p>
        </div>
        <!-- Grid column -->

      </div>
      <!--Grid row-->

    </div>
  </div>
</div>
      <div class="md-layout">
      </div>
      <div class="section-examples">
        <div class="container-fluid text-center">
          <div class="md-layout">
            <div class="md-layout-item">
              <a href="#/portfolio" target="_blank">
                <img
                  :src="landing"
                  alt="Rounded Image"
                  class="img-raised rounded img-fluid"
                />
              </a>
              <md-button href="#/portfolio" class="md-simple md-success md-lg"
                >View Portfolio Page</md-button
              >
            </div>
            <div class="md-layout-item">
              <a href="#/about" target="_blank">
                <img
                  :src="profile"
                  alt="Rounded Image"
                  class="img-raised rounded img-fluid"
                />
              </a>
              <md-button href="#/about" class="md-simple md-success md-lg"
                >View About Page</md-button
              >
            </div>
          </div>
        </div>
      </div>
      <div class="section section-download" id="downloadSection">
        <div class="container">

          <div class="sharing-area text-center">
            <div class="md-layout">
              <div class="md-layout-item">
                <h3>Thank you for supporting me!</h3>
              </div>
            </div>

            <md-button href="https://github.com/NickBarros10"class="md-github"
              ><i class="fab fa-github"></i> Star</md-button
            >
            <md-button href="https://www.linkedin.com/in/nick-barros-88379718a/" class="md-facebook"
              ><i class="fab fa-linkedin"></i>Follow</md-button
            >
            <md-button href="mailto:nickbarros10@gmail.com" class="md-google"
              ><i class="far fa-envelope"></i> Send</md-button
            >
            
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BasicElements from "./components/BasicElementsSection";
import Navigation from "./components/NavigationSection";
import SmallNavigation from "./components/SmallNavigationSection";
import Tabs from "./components/TabsSection";
import NavPills from "./components/NavPillsSection";
import Notifications from "./components/NotificationsSection";
import TypographyImages from "./components/TypographyImagesSection";
import JavascriptComponents from "./components/JavascriptComponentsSection";
import { LoginCard } from "@/components";

export default {
  components: {
    BasicElements,
    Navigation,
    SmallNavigation,
    Tabs,
    NavPills,
    Notifications,
    TypographyImages,
    JavascriptComponents,
    LoginCard
  },
  name: "index",
  bodyClass: "index-page",
  props: {
    image: {
      type: String,
      default: require("@/assets/img/vue-mk-header.jpg")
    },
    leaf4: {
      type: String,
      default: require("@/assets/img/leaf4.png")
    },
    leaf3: {
      type: String,
      default: require("@/assets/img/leaf3.png")
    },
    leaf2: {
      type: String,
      default: require("@/assets/img/leaf2.png")
    },
    leaf1: {
      type: String,
      default: require("@/assets/img/leaf1.png")
    },
    signup: {
      type: String,
      default: require("@/assets/img/city.jpg")
    },
    landing: {
      type: String,
      default: require("@/assets/img/landing.jpg")
    },
    profile: {
      type: String,
      default: require("@/assets/img/profile.jpg")
    }
  },
  data() {
    return {
      firstname: null,
      email: null,
      password: null,
      leafShow: false
    };
  },
  methods: {
    leafActive() {
      if (window.innerWidth < 768) {
        this.leafShow = false;
      } else {
        this.leafShow = true;
      }
    }
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.image})`
      };
    },
    signupImage() {
      return {
        backgroundImage: `url(${this.signup})`
      };
    }
  },
  mounted() {
    this.leafActive();
    window.addEventListener("resize", this.leafActive);
  },
  beforeDestroy() {
    window.removeEventListener("resize", this.leafActive);
  }
};
</script>
<style lang="scss">
.section-download {
  .md-button + .md-button {
    margin-left: 5px;
  }
}
.title{
  text-align: center;
}

@media all and (min-width: 991px) {
  .btn-container {
    display: flex;
  }
}
</style>
