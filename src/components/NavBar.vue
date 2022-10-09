<template>
  <div id="nav">
    <div class="nav-container">
      <div class="logo">
        <img id="logoPortifolio" src="../../public/logo/logo.svg" alt="">
      </div>
      <div class="links">
        <a href="#sobreMin">Sobre</a>
        <a href="#skills">Skills</a>
        <a href="#projetos">Projetos</a>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: 'NavBar',
}
</script>


<style scoped>
  @keyframes bounce {
    0% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-10px);
    }
    100% {
      transform: translateY(0);
    }
  }
    
  #nav{
  width: 100%;
  height: 100%;
  background: linear-gradient(0, #514b91, #120c56);
  overflow: hidden;
  }

  .nav-container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: auto;
    margin: 0 auto;
  }

  #logoPortifolio{
    width: 70px;
  }

  .links{
    display: flex;
    justify-content: space-between;
    align-items: center;    
    margin-right: 15px;
  }

  .links a:hover{
    animation: bounce 1s;
  }

 a{
  color: #fff;
  text-decoration: none;
  font-size: 1.2rem;
  padding: 0 10px;
  transition: all 0.3s ease;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  }

  .links a:hover{
    color: #000;
  }

</style>