<template>
  <div id="app">
    <Name/>
    <MainContent/>
    <About
      @openModal="isOpen = true"
      :isOpen="this.isOpen"
    />
    <transition
      name="fade"
      @after-enter="showContent = true"
    >
      <modal
        v-if="isOpen"
        @close="isOpen = false"
        @hideContent="showContent = false"
        :showContent="this.showContent"
      />
    </transition>
  </div>
</template>

<script>
import Name from './components/Name.vue'
import MainContent from './components/MainContent.vue'
import About from './components/About.vue'
import Modal from './components/Modal'

export default {
  name: 'app',
  components: {
    Name,
    MainContent,
    About,
    Modal
  },
  data: function(){
    return {
      isOpen: false,
      showContent: false
    }
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
    box-sizing: border-box;
}
#app {
  padding: 0 2rem;
  background: #e57373;
  height: 100vh;
  display: flex;
  flex-direction: row;
  flex-flow: nowrap;
}

a, abbr, acronym, address, applet, big, blockquote, body, button, caption, cite, code, dd, del, dfn, div, dl, dt, em, fieldset, font, form, h1, h2, h3, h4, h5, h6, html, iframe, img, ins, kbd, label, legend, li, object, ol, p, pre, q, s, samp, small, span, strike, strong, sub, sup, table, tbody, td, tfoot, th, thead, tr, tt, ul, var {
    font-family: Poppins,Helvetica,Arial,sans-serif;
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

.main-content {
  font-size: 2.5rem;
}

.fade-enter, .fade-leave-to {
  opacity: 0;
}
.fade-enter-active, .fade-leave-active {
  transition: 0.2s opacity ease-out;
}
</style>
