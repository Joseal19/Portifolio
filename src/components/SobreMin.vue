<template>
  <div class="container-forme">
    <div id="forMe" class="forMe-container">
      <div class="forMe">
        <div class="SobreMim">
          <div class="Me-img">
            <img id="img" src="../../public/img/ForMe.png" alt="">
          </div>
        </div>
      </div>
    </div>
    <div class="texto-container">
      <div class="textos">
        <div class="SobreMim">
          <div id="descricao">
            <h1 id="apresentacao">Me chamo José Alberto, sou um desenvolvedor Junior.</h1>
            <br>
            <div id="linha-horizontal"></div>
            <br>
            <h2>Atualmente estou cursando Ciência da Computação - UTFPR.</h2>
            <h2 id="apresentacao2">Estou em busca de novos conhecimentos e sempre disposto a aprender coisas novas.</h2>
            <h2>Desenvolvo aplicações com foco em Front-end, adoro desenvolver projetos prontos para o uso direto.
            </h2>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default{
    name: 'SobreMin',
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
    font-family: "Josefin Sans";
  }
  
  #descricao{
    padding-top: 12px;
    text-align: center;
  }

  #img{
    width: 100%;
    height: 100%;
    border-radius: 70%;
  }

  #linha-horizontal{
    width: 100%;
    height: 1px;
    background-color: black;
  }

  .texto-container{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
  }
  .textos{
    width: 50%;
    height: 320px;
    padding-top: 12px;
    text-align: center;
  }

  #apresentacao2, h2{
    text-align: center;
  }
.forMe-container{
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 100px;
  }

  @media screen and (min-width: 1920px){
    .forMe-container{
      padding-top: 131px;
    }
  }

  .forMe{
    scroll-behavior: smooth;
  }

</style>