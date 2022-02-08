<template>
  <div class="bg-lightblue">
    <div class="container">
      <ul class="d-flex">
        <li v-for="(image,index) in images" :key="index" class="d-flex">
          <img
            :src="require(`../../assets/img/${image.url}`)"
            :alt="image.alt"
          />
          <a href="#">{{image.text}}</a>
        </li> 
       
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainFooter",
  data(){
    return {
      images:[{
        url: "buy-comics-digital-comics.png",
        alt: "Digital Comics",
        text: "DIGITAL COMICS",
      },

      {
        url: "buy-comics-merchandise.png",
        alt: "Merchandise",
        text: "DC MERCHANDISE",
      },

      {
        url: "buy-comics-subscriptions.png",
        alt: "Subscriptions",
        text: "SUBSCRIPTION",
      },

      {
        url: "buy-comics-shop-locator.png",
        alt: "Shop Locator",
        text: "COMIC SHOP LOCATOR",
      },

      {
        url: "buy-dc-power-visa.svg",
        alt: "Digital Comics",
        text: "DC POWER VISA",
      },     


      ],
    }
  }
};
</script>

<style scoped>
.d-flex {
  display: flex;
}
.bg-lightblue {
  background-color: dodgerblue;
}
ul {
  padding: 50px 0;
  justify-content: center;
}

li {
  display: flex;
  justify-content: center;
  align-items: center;
}

a {
  text-decoration: none;
  color: white;
  font-size: 12px;
  margin: 0 30px;
}

img {
  height: 50px;  
}
</style>
