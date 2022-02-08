<template>
  <div class="bg-bottomfooter">
      <div class="container">
          <div class="row">
              <div class="col-3">
                <h4 id="sign">SIGN-UP NOW!</h4>
              </div>
              <div class="col-9">
                  <h4 id="follow">FOLLOW US</h4>
                  <ul>
                      <li><img src="../../assets/img/footer-facebook.png" alt="Facebook"></li>
                      <li><img src="../../assets/img/footer-twitter.png" alt="Twitter"></li>
                      <li><img src="../../assets/img/footer-youtube.png" alt="YouTube"></li>
                      <li><img src="../../assets/img/footer-pinterest.png" alt="Pinterest"></li>
                      <li><img src="../../assets/img/footer-periscope.png" alt="Periscope"></li>                                           
                  </ul>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:'BottomFooter',
}
</script>

<style scoped>
.bg-bottomfooter{
    background-color:#303030;
}

.row{
    display: flex;
    padding: 30px 0;
    justify-content:space-between;
}

#sign{
    padding: 15px 10px;
    border: 3px solid #1168b8;
    color: white;
}

#follow{
    color: dodgerblue;
}

.col-9{
    display: flex;
    align-items:center;    
}
ul{
    display: flex;
    list-style-type: none;
    padding: 0 20px;
}
li{
    padding: 0 10px;
}

</style>