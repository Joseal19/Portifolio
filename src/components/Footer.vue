<template>
  <div id="nav">
    <div class="footer-container">
      <p><a>Designed and developed by José Alberto <br><p><a> © 2022 Copyright</a></p></a></p>
      
    </div>
  </div>
</template>


<script>
export default {
  name: 'Footer',
}
</script>


<style scoped>
 
    
  #nav{
  width: 100%;
  height: 100%;
  background: linear-gradient(0, #514b91, #120c56);
  overflow: hidden;
  }

  .footer-container{
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: auto;
    margin: 0 auto;
  }

  p{
    color: #fff;
    font-size: 20px;
    text-align: center;
  }

  a{
    color: #fff;
    text-decoration: none;
    font-size: 1.2rem;
    padding: 0 10px;
  }

  p a{
    color: #fff;
    font-size: 15px;
    text-align: center;
  }
  

</style>