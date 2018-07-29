<template>
<div>
  <div>
    <div id="top">
      <div id="header">
        <div class="logo">
          <div class="pz-logo">
            PZ
          </div>
          <div class="pz-logo-caption">
            Paweł Zych
          </div>
        </div>
        <div class="header-title">
          <div>
            TRENER
          </div>
          <div>
            PERSONALNY
          </div>
        </div>
        <div class="header-place">
          <svg class="icon-place" viewBox="0 0 20 20">
							<path d="M10,1.375c-3.17,0-5.75,2.548-5.75,5.682c0,6.685,5.259,11.276,5.483,11.469c0.152,0.132,0.382,0.132,0.534,0c0.224-0.193,5.481-4.784,5.483-11.469C15.75,3.923,13.171,1.375,10,1.375 M10,17.653c-1.064-1.024-4.929-5.127-4.929-10.596c0-2.68,2.212-4.861,4.929-4.861s4.929,2.181,4.929,4.861C14.927,12.518,11.063,16.627,10,17.653 M10,3.839c-1.815,0-3.286,1.47-3.286,3.286s1.47,3.286,3.286,3.286s3.286-1.47,3.286-3.286S11.815,3.839,10,3.839 M10,9.589c-1.359,0-2.464-1.105-2.464-2.464S8.641,4.661,10,4.661s2.464,1.105,2.464,2.464S11.359,9.589,10,9.589"></path>
						</svg>
          Kalisz
        </div>
      </div>
      <ul id="menu">
          <li data-menuanchor="page1" class="active"><a href="#page1">Start</a></li>
          <li data-menuanchor="page2"><a href="#page2">Treningi</a></li>
          <li data-menuanchor="page3"><a href="#page3">Etapy</a></li>
          <li data-menuanchor="page4"><a href="#page4">Opinie</a></li>
          <li data-menuanchor="page5"><a href="#page5">Cennik</a></li>
          <li data-menuanchor="page6"><a href="#page6">Kontakt</a></li>
          <li>
            <a href="http://www.facebook.com/trenerpersonalnykalisz" target="_blank" title="Facebook">
                <svg class="icon-facebook" viewBox="0 0 512 512"><path d="M211.9 197.4h-36.7v59.9h36.7V433.1h70.5V256.5h49.2l5.2-59.1h-54.4c0 0 0-22.1 0-33.7 0-13.9 2.8-19.5 16.3-19.5 10.9 0 38.2 0 38.2 0V82.9c0 0-40.2 0-48.8 0 -52.5 0-76.1 23.1-76.1 67.3C211.9 188.8 211.9 197.4 211.9 197.4z"/></svg>
            </a>
          </li>
      </ul>
    </div>

    <full-page :options="options" @after-load="afterLoad" id="fullpage">
      <div class="section section-1">
        <div class="section__header">Twój sukces to mój sukces!</div>
        <div class="section__content">
          <div class="section__content__text">
            Tekst tutaj...
          </div>
        </div>
      </div>
      <!-- <div class="section">
        <div class="slide">
           <h3>Slide 2.1</h3>
        </div>
        <div class="slide">
           <h3>Slide 2.2</h3>
        </div>
        <div class="slide">
           <h3>Slide 2.3</h3>
        </div>
      </div> -->
      <div class="section section-2">
         <div class="section__header">Dopasowuję trening odpowiednio do Twoich potrzeb</div>
         <div class="section__content">
           <div class="section__content__text">
             Tekst tutaj...
           </div>
         </div>
      </div>
      <div class="section section-3">
         <div class="section__header">Prowadzę Cię do wymarzonej sylwetki i doskonałej formy</div>
         <div class="section__content">
           <div class="section__content__text">
             Tekst tutaj...
           </div>
         </div>
      </div>
      <div class="section section-4">
         <div class="section__header">Moją wizytówką są zadowoleni klienci</div>
         <div class="section__content">
           <div class="section__content__text">
             Tekst tutaj...
           </div>
         </div>
      </div>

      <div class="section section-5">
         <div class="section__header">Dostajesz ode mnie pierwszy trening za darmo</div>
         <div class="section__content">
           <div class="section__content__text">
             Tekst tutaj...
           </div>
         </div>
      </div>

      <div class="section section-6">
         <div class="section__header">Czekam na wszystkie Twoje pytania</div>
         <div class="section__content">
           <div class="section__content__text">
             Tekst tutaj...
           </div>
         </div>
      </div>
    </full-page>
  </div>
  <div id="loading-screen" v-bind:loaded="this.loaded">
    <div id="loading" class="loading__container">
      <div class="loading__circle">
        <div class="loading__circle__inside">
        </div>
        <div class="loading__rectangle1">
        </div>
        <div class="loading__rectangle2">
        </div>
        <div class="loading__shadow">
        </div>
      </div>
      <div class="loading__weights__container">
        <div class="loading__weights">
          <div class="w1 wl">
          </div>
          <div class="w2">
          </div>
          <div class="w3">
          </div>
          <div class="w4">
          </div>
          <div class="w5">
          </div>
          <div class="w6">
          </div>
          <div class="w5">
          </div>
          <div class="w4">
          </div>
          <div class="w3">
          </div>
          <div class="w2">
          </div>
          <div class="w1 wr">
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import FullPage from './assets/FullPage.vue'
import fullPageMixin from './assets/fullPageMixin'

export default {
  name: 'app',
  mixins: [fullPageMixin],
  components: {
    FullPage
  },
  data() {
      return {
        loaded: false,
        options: {
          afterLoad: this.afterLoad,
          scrollBar: false,
          menu: '#menu',
          navigation: true,
          anchors: ['page1', 'page2', 'page3', 'page4', 'page5', 'page6'],
          sectionsColor: ['#41b883', '#ff5f45', '#0798ec', '#fec401', '#1bcee6', '#ee1a59', '#2c3e4f', '#ba5be9', '#b4b8ab']
        },
      }
  },
  methods: {
      afterLoad() {
        // console.log("Emitted 'after load' event.");
        let self = this;
        setTimeout(function () {
          self.loaded = true;
        }, 2000);
      },

      toggleNavigation: function(){
            this.options.navigation = !this.options.navigation;
      }
    }
}
</script>

<style type="text/css">
@font-face {
    font-family: roboto;
    src: url(assets/fonts/Roboto-Regular.ttf);
}

@font-face {
    font-family: pz;
    src: url(assets/fonts/ftb.ttf);
}

blockquote, body, dd, div, dl, dt, fieldset, form, h1, h2, h3, h4, h5, h6, input, li, ol, p, pre, td, textarea, th, ul {
  padding: 0;
  margin: 0
}

a {
  text-decoration: none
}

table {
  border-spacing: 0
}

fieldset, img {
  border: 0
}

address, caption, cite, code, dfn, em, strong, th, var {
  font-weight: 400;
  font-style: normal
}

strong {
  font-weight: 700
}

ol, ul {
  list-style: none;
  margin: 0;
  padding: 0
}

caption, th {
  text-align: left
}

h1, h2, h3, h4, h5, h6 {
  font-weight: 400;
  font-size: 100%;
  margin: 0;
  padding: 0
}

q:after, q:before {
  content: ''
}

abbr, acronym {
  border: 0
}

* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box
}

body {
  font-family: roboto
}

.section {
  position: relative;
  background-size: cover;
  background-position: center center;
}

#section-1 {
  text-align: center
}

#section-1 h2:before {
  content: '';
  display: inline-block;
  height: 200px;
  width: 232px;
  background-image: url(assets/logo.png);
  background-repeat: no-repeat;
  background-size: cover;
  vertical-align: bottom
}

#section-1 h2 {
  color: #fff;
  font-size: 10em;
  font-weight: 900
}

#section-1 h1 {
  font-size: 2em;
  font-weight: 100;
  -webkit-font-smoothing: antialiased;
  -moz-font-smoothing: antialiased;
  margin: 1.5em auto 1em auto;
  color: #35495e;
  padding-right: 30px;
  padding-left: 30px
}

#section-1 li {
  display: inline-block;
  margin: 1.25em .3em
}

.section-1-button {
  padding: .93em 1.87em;
  background: #35495e;
  border-radius: 5px;
  display: block;
  color: #fff
}

h3 {
  font-size: 2.5em;
  text-align: center;
  color: #fff;
  font-weight: 700
}

#logo {
  position: fixed;
  top: 20px;
  left: 20px;
  color: #fff;
  font-weight: 700;
  z-index: 99;
  font-size: 1.9em;
  -webkit-font-smoothing: antialiased;
  -moz-font-smoothing: antialiased
}

#menu-line {
  position: absolute;
  bottom: -4px;
  left: 0;
  width: 159px;
  height: 2px;
  background: #fff
}

#menu {
  z-index: 70;
  -webkit-font-smoothing: antialiased;
  -moz-font-smoothing: antialiased;
  letter-spacing: 1px;
  font-size: 1.1em;
  display: flex;
  align-items: center;
}

#menu li {
  display: inline-block;
  margin: 10px 0;
  position: relative
}

#menu a {
  color: #fff;
  padding: 0 0.8em 1.1em 0.8em
}

#menu li.active a:after {
  content: '';
  margin: 0 0.8em 0 0.8em;
  height: 2px;
  background: #fff;
  display: block;
  position: absolute;
  bottom: -6px;
  left: 0;
  right: 0;
  display: block
}

.actions {
  position: fixed;
  bottom: 2%;
  margin: 0 auto;
  z-index: 99;
  left: 0;
  right: 0;
  text-align: center
}

.actions li {
  display: inline-block;
  margin: .3em .3em
}

.actions-button {
  padding: .73em 1.47em;
  background: rgba(53, 73, 94, .47);
  border-radius: 5px;
  display: block;
  color: #fff
}

.icon-facebook {
  width: 32px;
  color: #fff;
  fill: #fff;
  border-color: #fff;
  border-width: 2px;
  border-style: solid;
  border-radius: 10px;
  position: relative;
  top: 3px;
}

.icon-place {
  width: 32px;
  color: #fff;
  fill: #fff;
}

#top {
  position: fixed;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  z-index: 100;
  padding: 10px 35px;
}

#header {
  width: 100%;
  color: #fff;
  display: flex;
  align-items: center;
}

.logo {

}

.pz-logo {
  font-family: pz;
  font-size: 93px;
  padding: 0;
  line-height: 0.6;
}

.pz-logo-caption {
  text-align: center;
  font-size: 16px;
  letter-spacing: 3px;
  position: relative;
  right: 4px;
  text-transform: uppercase;
}

.header-title {
  font-size: 28px;
  font-weight: 800;
  margin: 0 28px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-between;
  line-height: 1;
  height: 100%;
  padding-top: 6px;
}

.header-place {
  display: flex;
  align-items: center;
  font-size: 22px;
}

#loading-screen {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #000000;
  margin: 0;
  position: fixed;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: 300;
  transition-property: opacity;
  transition-duration: 800ms;
  transition-timing-function: ease-in;
  opacity: 1;
}

#loading-screen[loaded] {
  opacity: 0;
  pointer-events: none;
}

.loading__container {
  height: 200px;
  width: 200px;
  background-color: #000000;
  position: relative;
}

.loading__circle {
  width: 100%;
  height: 100%;
  background-color: #ffffff;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  animation-name: loading;
  animation-duration: 1s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}

.loading__circle__inside {
  background-color: #000000;
  width: 90%;
  height: 90%;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.loading__rectangle1 {
  background-color: #000000;
  width: 60%;
  height: 50%;
  position: absolute;
  top: 0;
  left: 0;
}

.loading__rectangle2 {
  background-color: #000000;
  width: 100%;
  height: 10%;
  position: absolute;
  top: 0;
}

.loading__shadow {
  background: linear-gradient(to bottom, black, rgba(0,0,0,0));
  width: 40%;
  height: 40%;
  position: absolute;
  top: 10%;
  right: 0;
}

.loading__weights__container {
  position: absolute;
  top: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.loading__weights {
  width: 90%;
  height: 90%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.loading__weights > div {
  background-color: #ffffff;
  z-index: 1;
}

.loading__weights > .w1 {
  width: 5%;
  height: 6%;
}

.loading__weights > .w2 {
  width: 3%;
  height: 9%;
  border-radius: 1px;
}

.loading__weights > .w3 {
  width: 7%;
  height: 30%;
  border-radius: 3px;
}

.loading__weights > .w4 {
  width: 8%;
  height: 40%;
  border-radius: 3px;
}

.loading__weights > .w5 {
  width: 3%;
  height: 9%;
  border-radius: 1px;
}

.loading__weights > .w6 {
  width: 40%;
  height: 6%;
}

.loading__weights > .wl {
  border-top-left-radius: 2px;
  border-bottom-left-radius: 2px;
}

.loading__weights > .wr {
  border-top-right-radius: 2px;
  border-bottom-right-radius: 2px;
}

@keyframes loading {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

.section-1 {
  background-image: url('assets/background1.jpg');
}

.section-2 {
  background-image: url('assets/background2.jpg');
}

.section-3 {
  background-image: url('assets/background3.jpg');
}

.section-4 {
  background-image: url('assets/background5.jpg');
}

.section-5 {
  background-image: url('assets/background4.jpg');
}

.section-6 {
  background-image: url('assets/background6.jpg');
}

#fp-nav > ul > li > a > span {
  background-color: #a5a5a5;
}

.section__header {
  text-align: center;
  color: #ffffff;
  font-size: 2.5em;
  font-weight: 800;
}

.section__content {
  display: flex;
  align-items: center;
  justify-content: center;
}

.section__content__text {
  width: 50%;
  margin-top: 1em;
  color: #ffffff;
  text-align: center;
}
</style>
