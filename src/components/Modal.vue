<template>

    <div
      class="modal"
      @click="$emit('hideContent')"
    >
      <transition
        name="content"
        @after-leave="$emit('close')"
      >
        <div
          v-if="showContent"
          class="content"
          @click.stop
        >
        <h1>Je suis disponible pour un stage ou en freelance</h1>
        <p>
          A l'écoute pour un poste junior sur le langage PHP. 
        </p>

        </div>
      </transition>
    </div>

</template>

<script>
export default {
  props: {
    showContent: Boolean
  }
}
</script>

<style scoped>
/*
.about-container {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 99;
  width: 100%;
  height: 100%;
  overflow: hidden;
  display: none
}
.about-overlay {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 98;
  background: #000;
  opacity: 0;
  width: 100%;
  height: 100%
}

@media (min-width:960px) {
  .about-overlay {
    background: rgba(0, 0, 0, 0)
  }
}

.about-container .about-wrapper {
    position: absolute;
    bottom: 0;
    right: 0;
    z-index: 99;
    background: #fbfaf7;
    width: 95%;
    height: 88%;
    -webkit-transform: translateY(100%);
    -ms-transform: translateY(100%);
    transform: translateY(100%);
    overflow: scroll;
    -webkit-overflow-scrolling: touch
}

@media (min-width:960px) {
    .about-container .about-wrapper {
        overflow: auto;
        -webkit-overflow-scrolling: initial;
        width: 96.09375%;
        height: 91.52941%
    }
}
*/

.modal {
  position: absolute;
  overflow: hidden;
  top: 0;
  left: 0;
  right: 0;
  width: 100vw;
  height: 100vh;
  background: rgba(0,0,0,0.6)
}
.content {
  position: absolute;
  bottom: 0;
  right: 0;
  z-index: 99;
  background: #fbfaf7;
  width: 89.5%;
  height: 86%;
  overflow: scroll;
  border-radius: 3px;
  font-style: normal;
  font-weight: 300;
  font-size: 16px;
  line-height: 26px;
  color: #000;
  letter-spacing: -.22px;
  padding: 20px;
  -webkit-overflow-scrolling: touch
}
.content > p {
  color: #444;
}
.content-enter {
  transform: translateY(100%);
}

.content-leave-to {
  transform: translateY(100%);
}
.content-enter-active, .content-leave-active {
  transition: .4s;
}
</style>