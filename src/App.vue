<template>
  <div id="app">
    <MainNav></MainNav>
    <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <div class="home">
      <main-col/>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MainNav from './components/MainNav.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    MainNav,
  }
}
</script>

<style>
@import url('./assets/fonts/fonts.css');
* {
    vertical-align: baseline;
    border: 0;
    outline: 0;
    padding: 0;
    margin: 0;
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
}

a, abbr, acronym, address, applet, big, blockquote, body, button, caption, cite, code, dd, del, dfn, div, dl, dt, em, fieldset, font, form, h1, h2, h3, h4, h5, h6, html, iframe, img, ins, kbd, label, legend, li, object, ol, p, pre, q, s, samp, small, span, strike, strong, sub, sup, table, tbody, td, tfoot, th, thead, tr, tt, ul, var {
    /*font-family: Poppins,Helvetica,Arial,sans-serif;*/
    color: #2b2d30;
    font-family: 'Poppins', sans-serif;
    font-size: 1.4rem;
    line-height: 1.8;
    letter-spacing: .01em;
    font-weight: 400;
    font-style: normal;
    vertical-align: baseline;
    border: 0;
    outline: 0;
    padding: 0;
    margin: 0;
}
.home {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
    -ms-flex-direction: row;
    flex-direction: row;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    -webkit-box-flex: 0;
    -ms-flex: 0 1 auto;
    flex: 0 1 auto;
    flex-grow: 0;
    flex-shrink: 1;
    flex-basis: auto;
}

.main-content {
  font-size: 2.5vw;
}
</style>
