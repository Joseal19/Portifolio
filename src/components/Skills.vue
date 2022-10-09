<template>
  <div class="container">
    <p id="titulo">Skills</p> 
    <div id="skills">
      <table>
        <caption id="titulo-table">Front-end</caption>
        <tr>
          <td>
            <p>HTML</p>
            <p>Java Script</p>
            <p>Vue</p>
            <p>React</p>
          </td>
        </tr>
      </table>
      <br>
      <table> 
        <caption id="titulo-table">Back-end</caption>
        <tr>
          <td>
            <p>PHP</p>
            <p>Jquery</p>
            <p>Node</p>

          </td>
        </tr>
      </table>
      </div>
  </div>
</template>

<script>
  export default {
    name: 'Skill',
  };

</script>

<style scoped>

  #skills {
    animation: go-back 7s;
    animation-iteration-count: 1;
  }

  @keyframes go-back {
    from {
      transform: translateX(1200px);
    }
    to {
      transform: translateX(0);
    }
  } 


  @media screen and (min-width: 1920px){
    .container{
      padding-top: 150px;
      padding-bottom: 12px;
    }
  }

  #titulo{
    text-align: center;
    font-size: 30px;
    padding-top: 20px;
  } 

  #skills{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
  }

  table{
    width: 100%;
    height: 100%;
  }

  td{
    width: 100%;
    height: 100%;
    text-align: center;
    font-size: 20px;
  }

  td p{
    padding: 10px;
  }

  
  #titulo{
    font-size: 50px;
    text-align: center;
    padding: 50px 0;
  }

  #titulo-table{
    font-size: 30px;
    text-align: center;
    padding: 50px 0;
    position: relative;
    font-family: fantasy;
  }


  
  #img{
    border-radius: 50px;
    width: 100%;
    height: 100%;
  }
  .skills-container{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
  
  .skills{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
  }

  .skill{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 100px;
    height: 100px;
    margin: 10px;
    border-radius: 50%;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0,0,0,0.5);
  }

  .skill:hover{
    -webkit-transform: scale(1.3);
    -ms-transform: scale(1.3);
    transform: scale(1.3);
  }
  .skill img{
    width: 50px;
    height: 50px;
    margin-top: 10px;
  }
  .skill p{
    margin-top: 10px;
  }


</style>