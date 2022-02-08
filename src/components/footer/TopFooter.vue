<template>
  <div class="background-image">
    <div class="container">
      <div class="row">

        <div class="col">
          <h4>DC COMICS</h4>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Video</li>
            <li>News</li>
          </ul>
          <h4>SHOP</h4>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>

        <div class="col">
          <h4>DC</h4>
          <ul>
            <li>Terms Of Use</li>
            <li>Privacy policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
        </div>

        <div class="col">
          <h4>SITES</h4>
          <ul>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </div>

        <div class="col" id="dc-logo">
          
        </div>        
      </div>      
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.background-image{
  background-image:url('../../assets/img/footer-bg.jpg');  
}

#dc-logo{
  background-image:url('../../assets/img/dc-logo-bg.png');
  height:450px;
  width:100%;
  background-repeat: no-repeat;
  background-position: center;
}

.row {
  display: flex;
  padding: 30px 0; 
}
h4 {
  padding: 20px 0;
  font-weight: bold;
  color:white;
}

li {
  list-style-type: none;
  padding: 5px 0;
  font-size: 13px;
  color: white;
}

.col {
  margin-right: 50px;  
}
</style>
