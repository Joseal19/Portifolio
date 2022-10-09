<template>
  <div>
   <Home />
    <button id="ceta">
      <a href="#sobreMin" class="ceta">
        <img class="ceta" src="../public/img/ceta.png" alt="">
      </a>
    </button>
    <div id="buttons">
      <button id="conta1">
        <a href="https://www.linkedin.com/in/josealbertonp/" class="conta1" target="_blank">
          <img class="conta1" src="../public/img-contato/linkedin.png" >
        </a>
      </button>
      <button id="conta2">
        <a href="https://github.com/Joseal19" class="conta2" target="_blank">
          <img class="conta2" src="../public/img-contato/github.png" >
        </a>
      </button>
      <button id="conta3">
        <a href="mailto:contato@josealbertonp.com" class="conta3" target="_blank">
          <img class="conta3" src="../public/img-contato/email.png" >
        </a>
      </button>
    </div>
  </div>
</template>

<script>
  import Home from './views/Home.vue';

export default {
    components: {
      Home
    },
}
</script>

<style>

  *{
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  #ceta{
    position: fixed;
    bottom: 0;
    right: 0;
    margin: 20px;
    border: none;
    background-color: transparent;
    cursor: pointer;
  }

  #ceta{
    color: #fff;
    font-size: 30px;
    text-decoration: none;
    transition: 0.5s;
  }

  .ceta{
    width: 50px;
    height: 50px;
    border-radius: 28px;
  }

  #ceta:hover{
    transform: scale(1.1);
  }

  #buttons{
    position: fixed;
    bottom: 0;
    right: 0;
    margin: 20px;
    display: flex;
    flex-direction: column;
    background-color: black; 
    align-items: flex-end;
  }

  #conta1, #conta2, #conta3{
    position: fixed;
    bottom: 50%;
    right: 90%;
    border: none;
    background-color: transparent;
    cursor: pointer;
  }

  @media screen and (min-width: 1920px){
    #conta1, #conta2, #conta3{
      margin-bottom: 50px;
    }
  }

  #conta2{
    bottom: 40%;
  }

  #conta3{
    bottom: 30%;
  }

  #conta1, #conta2 , #conta3{
    color: #fff;
    font-size: 30px;
    text-decoration: none;
    
  }

  .conta1, .conta3{
    width: 50px;
    height: 50px;
  }

  .conta2{
    width: 55px;
    height: 55px;
  }

  .conta3{
    margin-right: 1.5px;
    margin-bottom: 5px;
  }

  #conta1:hover, #conta2:hover, #conta3:hover{
    transform: scale(1.1);
  }


  @media screen and (max-width: 5700px){
    #buttons{
      background-color: black;
    }
  }


</style>
