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
}
</script>
<style scoped>
@media (min-width: 960px){
  #main-nav {
    padding: 23px 35px;
  }
}
#main-nav {
    position: absolute;
    z-index: 99;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
    -ms-flex-direction: row;
    flex-direction: row;
    justify-content: space-between;
    -webkit-box-align: start;
    -ms-flex-align: start;
    align-items: flex-start;
    width: 100%;
    top: 0;
    left: 0;
    pointer-events: none;
    padding: 14px 20px;
}
.flex-row {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  align-items: center;
}
.name {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding-left: 4.5rem;
}
.dot {
    display: inline-block;
    background-color: #000;
    border-radius: 100%;
    width: 12px;
    height: 12px;
    -webkit-transform: scale(0);
    -ms-transform: scale(0);
    transform: scale(0);
}
.firstname {
    font-size: 16px;
    letter-spacing: 4px;
    margin-left: 0.5rem;
    line-height: 30px;
    font-weight: 400;
    font-style: normal;
    color: #4a5568;
    text-transform: uppercase;
}
.lastname {
  font-size: 20px;
  margin-top: -4px;
  line-height: 18px;
  letter-spacing: 0.12em;
  text-transform: uppercase;
}
button {
    font-family: Poppins,Helvetica,Arial,sans-serif;
    font-weight: 400;
    font-style: normal;
    font-size: 16px;
    color: #000;
    letter-spacing: .23px;
    text-align: right;
    -webkit-transition: color .3s ease-in-out;
    -o-transition: color .3s ease-in-out;
    transition: color .3s ease-in-out;
}
</style>


