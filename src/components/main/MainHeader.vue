<template>
  <div>
    <section class="bg-image"></section>
    <section class="bg-black">
      <div class="container pos-relative">

        <button class="pos-absolute">CURRENT SERIES</button>

        <div class="cards">
          <div v-for="(product, index) in products" :key="index" class="card">
            <figure>
              <img :src="product.thumb" :alt="product.series" />
            </figure>            
            <h4>{{ product.series.toUpperCase() }}</h4>
          </div>
        </div>
        <div class="center-button">
          <button>LOAD MORE</button>
        </div>

      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "MainHeader",
  props: ["products"]
};
</script>

<style lang="scss" scoped>
.bg-black {
  background-color: #1c1c1c;
}
.bg-image {
  background-image: url(../../assets/img/jumbotron.jpg);
  min-height: 400px;
  background-size: cover;
}
button {
  padding: 10px 20px;
  background-color: dodgerblue;
  color: white;
  font-weight: bold;
  font-size: 20px;
  cursor: pointer;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  padding-top:50px;  

  .card {    
    flex-basis: calc(100% / 6);
    padding:10px;

    figure{
       overflow: hidden;
      width:180px;
      height:180px;
    }   

    h4 {
      color: white;
      padding-top: 20px;
    }
  }
}

.center-button{
  display: flex;
  justify-content: center;
  padding:20px 0;
}

.pos-relative{
  position: relative;
}

.pos-absolute{
  position: absolute;
  top:-25px;
  left:0;
}
</style>
