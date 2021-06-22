<template>
  <div id="app">

    <Header :navArr="navLinks"/>

    <Main />

    <Footer  :footOne="cardOne" :footTwo="cardTwo" :footThree="cardThree" :footFour="cardFour"/>
   
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import "../src/style/general.scss"

export default {
  name: 'App',
      data() {
        return {
            navLinks: [
                {
                  txt: "home",
                  active: true 
                },
                {
                  txt: "about",
                  active: false
                },
                {
                  txt: "service",
                  active: false
                },
                {
                  txt: "team",
                  active: false
                },
                {
                  txt: "blog",
                  active: false
                },
                {
                  txt: "",
                  active: false
                },
                {
                  txt: "get in touch",
                  active: false
                }
            ],
            cardOne: [
            "A Functional HTML template for Business and Corporate", 
            "123456789",
            "mail@mail.com",
            "Location via 123"
            ],
            cardTwo: [
              "the company",
              "institutional",
              "social & events",
              "innovation",
              "Enviroment",
              "technology"
            ],
            cardThree:[
              "audit & assurance",
              "financial advisoty",
              "analytics M&A",
              "middle marketing",
              "legal consulting",
              "regulatory risk"
            ],
            cardFour: [
              "responsability",
              "term of use",
              "about cookies",
              "privacy policy",
              "accessibility",
              "information"
            ]
        }
    },
  components: {
    Header,
    Main,
    Footer
  }

}
</script>

<style lang="scss">
// @import "../style/vars.scss";

</style>
