<template>
  <div class="background-image">
    <div class="container">
      <div class="row">

        <div class="col">
          <h4>DC COMICS</h4>
          <ul>
            <li v-for="(comic,index) in comics" :key="index">{{comic.text}}</li>            
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
            <li v-for="(ud,index) in ud" :key="index">{{ud.text}}</li>              
          </ul>
        </div>

        <div class="col">
          <h4>SITES</h4>
          <ul>
            <li v-for="(site,index) in sites" :key="index">{{site.text}}</li>   
          </ul>
        </div>

        <div class="col" id="dc-logo"></div>        
      </div>      
    </div>
  </div>
</template>

<script>
export default {
  name:'TopFooter',
  data(){
    return {
      comics: [{
        text: "Characters",
        active: true,
      },
      {
        text: "Comics",
        active: false,
      },
      {
        text: "Movies",
        active: false,
      },
      {
        text: "TV",
        active: false,
      },
      {
        text: "Video",
        active: false,
      },
      {
        text: "News",
        active: false,
      },     
      ],


      /* UD */


       ud: [{
        text: "Terms Of Use",
        active: true,
      },
      {
        text: "Privacy policy (New)",
        active: false,
      },
      {
        text: "Ad Choices",
        active: false,
      },
      {
        text: "Advertising",
        active: false,
      },
      {
        text: "Jobs",
        active: false,
      },
      {
        text: "Subscriptions",
        active: false,
      },     
      {
        text: "Talent Workshops",
        active: false,
      },     
      {
        text: "CPSC Certificates",
        active: false,
      },     
      {
        text: "Ratings",
        active: false,
      },     
      {
        text: "Shop Help",
        active: false,
      },     
      {
        text: "Contact Us",
        active: false,
      },     
      ],


      /* SITES */


      sites: [{
        text: "DC",
        active: true,
      },
      {
        text: "MAD Magazine",
        active: false,
      },
      {
        text: "DC Kids",
        active: false,
      },
      {
        text: "DC Universe",
        active: false,
      },
      {
        text: "DC Power Visa",
        active: false,
      },     
      ],
    }
  }
};
</script>

<style scoped>
.background-image{
  background-image:url('../../assets/img/footer-bg.jpg');
  background-repeat:no-repeat;
  background-size:cover;  
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

.col{
  width: 200px;
  margin-right: 30px;
}

</style>
