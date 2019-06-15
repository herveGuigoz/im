<template>
  <div id="main-nav">
    <div class="name">
      <div class="flex-row">
        <span class="dot" style="transform: matrix(1, 0, 0, 1, 0, 0);"></span>
        <h1 class="firstname">Herve</h1>
      </div>
      <h1 class="lastname">Guigoz</h1>
    </div>
  <button>ABOUT</button>
  </div>
</template>
<script>
export default {
  name: 'MainNav',
  props: {
    showAbout: Boolean
  }
  }
}
</script>
<style scoped>
#main-nav {
  /*
    position: absolute;
    z-index: 99;
    */
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-start;
    width: 100%;
    top: 0;
    left: 0;
    padding: 1rem 2rem;
}

button {
    font-family: Poppins,Helvetica,Arial,sans-serif;
    font-weight: 400;
    font-style: normal;
    font-size: 16px;
    color: #4a5568;
    background: transparent;
    letter-spacing: .23px;
    text-align: right;
    /*
    -webkit-transition: color .3s ease-in-out;
    -o-transition: color .3s ease-in-out;
    transition: color .3s ease-in-out;
    */
}
</style>


