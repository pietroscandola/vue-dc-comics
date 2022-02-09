<template>
  <div class="bg-white">
    <div class="container">
      <header>
        <nav>
          <div class="row d-flex">
            <div class="col-left">
              <figure>
                <img src="../assets/img/dc-logo.png" alt="Logo DC" />
              </figure>
            </div>
            <div class="col-right">
              <ul class="d-flex">
                <li
                  v-for="(link, index) in links"
                  :key="index"
                  :class="{ active: link.active }"
                >
                  <a href="#">{{ link.text }}</a>
                </li>
              </ul>
            </div>
          </div>
        </nav>
      </header>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          active: true,
        },
        {
          text: "COMICS",
          active: false,
        },
        {
          text: "MOVIES",
          active: false,
        },
        {
          text: "TV",
          active: false,
        },
        {
          text: "GAMES",
          active: false,
        },
        {
          text: "COLLECTIBLES",
          active: false,
        },
        {
          text: "VIDEOS",
          active: false,
        },
        {
          text: "FANS",
          active: false,
        },
        {
          text: "NEWS",
          active: false,
        },
        {
          text: "SHOP",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>

img {
  width: 80%;
}
.bg-white {
  background-color: white;
}

.d-flex {
  display: flex;
}

.row {
  display: flex;
  justify-content: space-between;
  align-items:center;
}

.col-right {
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

.col-left figure {
  display: flex;
  justify-content: flex-start;
  align-items: start;
}

li {
  border-bottom: 5px solid transparent;
  list-style-type: none;
  font-size: 14px;
  font-weight: bold;
  padding: 60px 10px;

  &.active {
    color: dodgerblue;
    border-bottom: 5px solid dodgerblue;
  }
  a {
    color: black;
    text-decoration: none;
  }
}
</style>
