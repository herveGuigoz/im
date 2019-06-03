<template>
  <div id="main-content">
    <div class="me">
      <p>Passionné du numérique, je me suis réorienté vers le métier de <span class="white">développeur Web.</span><br> La formation à la Wild Code School de Lyon m’a permis de mettre en pratique la méthode Scrum à travers la réalisation de projets clients et de me perfectionner sur le framework PHP, Symfony.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainContent',
}
</script>

<style scoped>
#main-content {
  margin-top:4rem;
  width: 100vw;
  padding-left: 0;
  margin-left: 0;
}

p, span {
  font-size: 2.5vw;
  line-height: 4.21875vw;
  letter-spacing: -.4px;
  margin-top: 0;
  color: #4a5568;
  font-family: 'Poppins', sans-serif;
  line-height: 1.8;
  letter-spacing: .01em;
}

/* @media (max-width: 640px) { p,span {font-size:16px; line-height:30px;} } */

.white {
  color:#ffffff;
}
</style>
