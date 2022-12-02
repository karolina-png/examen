<template>
  <div id="container-fluid">
    <nav class="navbar navbar-expand-lg  bg-dark">
      <div class="container-fluid">
        <div>
          <router-link class="nav_item" to="/login"> <b>LOGIN</b> </router-link>
        </div>

      
      </div>
    </nav>
   
    <div id="container_main">





      <router-view>

      </router-view>







    </div>

  </div>




 

</template>
<style scoped>
  #container {
    display: flex;
    flex-direction: column;
    background-position: center;
    background-size: cover;
    width: 100vw;
    height: 100vh;
    


  }

  .navbar {
    display: flex;
    width: 100vw;
    height: 5rem;
    background-color: rgba(19, 2, 31, 0.829) !important;
    color: white;
    font-size: 3rem;
  }

  .container-fluid {
    display: flex;
    flex-direction: row;
    
    width: 100%;
   
  }

  .d-flex {
    display: flex;
    flex-direction: column;
    justify-content: center;
    /* border: 1px solid white; */

  }

  #d-flex {
    display: flex;
    flex-direction: row;
    height: max-content;
  }

  #d-flex button {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: max-content;
    font-size: 1rem;
    background-color: transparent !important;
    border: 1px solid white !important;
    color: white;
  }

  #d-flex button:hover {
    background-color: white !important;
    border: 1px solid white;
    color: black !important;
  }
  #d-flex button:active {
    transform: scale(0.95);
  }

  .btn {
    height: 2rem;
    /* border: 1px solid white; */
    margin: 2px;
    border-radius: 5px;
  }

  #container_main {
    display: flex;
    flex-direction: column;

    height: calc(100% - 7.5rem);
    width: 100%;
  
  }



  #sub_nav {

    display: flex;
   
    overflow-y: hidden;
    width: 100%;
    height: 2.7rem;
    background-color: white;
  }

  .subnav {
    display: flex;
    flex-direction: row;
    width: 100%;
  }

  .nav_item {
    display: flex;

    justify-content: center;
    font-size: 1.5rem;
    color: black;
    padding-left: 1rem;
    padding-right: 1rem;
    border: 1px solid black;
    border-radius: 5px;
    margin: 2px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    background-color: transparent;
    /* height: max-content; */
    transition: cubic-bezier(0.785, 0.135, 0.15, 0.86);

  }

  .nav_item:hover {
    background-color: white;
    color: white;
  }
  .nav_item:active{
    transform: scale(0.95);
  }
  h2{
    font-size: 3rem;
  }

  @media (max-width: 400px) {
   

   


  }
</style>
<script>

 
</script>