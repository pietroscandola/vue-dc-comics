<template>
  <div class="bg-lightblue">
      <ul class="d-flex">
          <li class="d-flex">
              <img src="..\..\assets\img\buy-comics-digital-comics.png" alt="Digital Comics">
              <a href="#">DIGITAL COMICS</a>            
          </li>
          <li>
              <img src="..\..\assets\img\buy-comics-merchandise.png" alt="Merchandise">
              <a href="#">DC MERCHANDISE</a>            
          </li>
          <li>
              <img src="..\..\assets\img\buy-comics-subscriptions.png" alt="Subscriptions">
              <a href="#">SUBSCRIPTION</a>            
          </li>
          <li>
              <img src="..\..\assets\img\buy-comics-shop-locator.png" alt="Shop Locator">
              <a href="#">COMIC SHOP LOCATOR</a>            
          </li>
          <li>
              <img src="..\..\assets\img\buy-dc-power-visa.svg" alt="Digital Comics">
              <a href="#">DC POWER VISA</a>            
          </li>         
      </ul>
  </div>
</template>

<script>
export default {
    name: 'MainFooter',
}
</script>

<style scoped>
.d-flex{
    display: flex;
}
.bg-lightblue{
    background-color:dodgerblue;    
}
ul{
    padding: 30px 0;
}

li{
    display:flex;
    justify-content:center;
    align-items:center;
}

a{
    text-decoration:none;
    color: white;
    font-size:12px;
    margin: 0 10px;
}

img{
    width:25%;
}

</style>