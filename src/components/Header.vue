<template>
  <div class="container">
      <header>
          <nav>
              <div class="row d-flex ">
                  <div class="col-left">
                      <figure>
                          <img src="../assets/img/dc-logo.png" alt="Logo DC">
                      </figure>
                  </div>
                  <div class="col-right">
                      <ul class="d-flex ">
                          <li class="active"><a href="#">CHARACTERS</a></li>
                          <li><a href="#">COMICS</a></li>
                          <li><a href="#">MOVIES</a></li>
                          <li><a href="#">TV</a></li>
                          <li><a href="#">GAMES</a></li>
                          <li><a href="#">COLLECTIBLES</a></li>
                          <li><a href="#">VIDEOS</a></li>
                          <li><a href="#">FANS</a></li>
                          <li><a href="#">NEWS</a></li>
                          <li><a href="#">SHOP</a></li>                                                    
                      </ul>
                  </div>                
              </div>
          </nav>
      </header>
  </div>
</template>

<script>
export default {
    name: 'Header',    
}
</script>

<style scoped>
img{
    width: 50%;
}

header{
    padding: 30px 0;
}

.d-flex {
    display: flex;
}

.row {
    display: flex;
    justify-content:space-between;
}

.col-right{
    display:flex;
    align-items: center;
    justify-content: flex-end;
}

.col-left figure{
    display:flex;
    justify-content: flex-start;
    align-items: start;
}


li{
    margin: 0 15px;
    list-style-type: none;
    font-size:14px;
    font-weight: bold;
    padding: 20px 0;   
}

li a {
   color: black;
   text-decoration:none;
   
}

.active {
    color: dodgerblue;
    border-bottom: 5px solid dodgerblue;    
}

</style>