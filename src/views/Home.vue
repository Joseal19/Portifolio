<template>
  <div>
    <div id="navBar">
      <NavBar />
    </div>
    <div id="sobreMin">
      <SobreMin />
    </div>
    <div class="container" id="skills">
        <Skills />
    </div>
    <div id="projetos">
      <Projetos />
    </div>
    <Footer />

  </div>
</template>

<script>
import NavBar from '../components/NavBar.vue';
import Projetos from '../components/Projetos.vue';
import SobreMin from '../components/SobreMin.vue';
import Skills from '../components/Skills.vue';
import Footer from '../components/Footer.vue';

  export default{
    name: 'Home',
    components: {
      NavBar,
      Projetos,
      SobreMin,
      Skills,
      Footer
    },
  }
</script>

<style>
  html{
    scroll-behavior: smooth;
  }
</style>

<style scoped>

  *{
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  } 
  @media screen and (min-width: 1920px){
    #sobreMin{
      padding-top: 150px;
      padding-bottom: 12px;
    }
  }
  
  #sobreMin{
    height: 100vh;
  }


  #skills{
    height: 100vh;
  }

  #projetos{
    padding: 9vh;
    height: 100vh;
  }
  
  #navBar{
    position: fixed;
    width: 100%;
  }

  @media screen and (max-width: 768px){
    #sobreMin{
      height: 120vh;
    }
  }

</style>