<template>
  <div>
    <p id="projetos">Projetos</p> 
    <div  class="projetos-container">
      <div class="projetos">
        <div class="projeto">
          <div class="projeto-img">
            <img src="../../public/img/Projeto1.png" alt="">
          </div>
          <div class="projeto-desc">
            <h2>Big Burguer</h2>
            <p>Uma pagina de pedidos simples e completa.</p>
            <a id="buttonProjeto" href="https://lanchonetebigburger.netlify.app/" target="_blank">Ler Mais</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

  export default{
    name: 'Projetos',
    components: {

    }
  }
</script>

<style scoped>
  *{
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  #projetos{
    font-size: 50px;
    text-align: center;
  }

  @media screen and (min-width: 1920px){
    #projetos{
    margin-top: 123px;
  }
  }

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

  .projetos-container{
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 71px;
  }

  #buttonProjeto{
    background-color: rgb(95, 82, 82);
    color: #fff;
    border-radius: 5px;
    text-decoration: none;
    transition: 0.5s;
    margin-bottom: 12px;
  }

  .projetos{
    display: flex;
    justify-content: space-between;
    align-items: center;
    display: flex;
    background-color: #fff;
    border-radius: 10px;
    width: 500px;
    box-shadow: 0 10px 10px rgba(0,0,0,0.2);
  }

  .projeto-img{
    /* height: 100%; */
    border-radius: 10px;
    overflow: hidden;
  }

  .projeto-img img{
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  .projeto-desc a:hover{
    animation: bounce 1s;
  }

  .projeto-desc{
    width: 50%;
    height: 100%;
    padding: 0 20px;
  }

  .projeto-desc h2{
    font-size: 1.5rem;
    font-weight: bold;
    margin-bottom: 10px;
  }

  .projeto-desc p{
    font-size: 1.2rem;
    color: #666;
  }

  .projeto-desc a{
    display: inline-block;
    width: 100px;
    height: 30px;
    background-color: rgb(95, 82, 82);
    color: #fff;
    text-decoration: none;
    text-align: center;
    line-height: 30px;
    border-radius: 5px;
    margin-top: 20px;
  }

  .projeto-desc a:hover{
    background-color: rgb(75, 60, 60);
  }
  
</style>