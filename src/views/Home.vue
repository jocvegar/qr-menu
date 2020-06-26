<template>
  <div class="home">
    <div class="jumbotron jumbotron-fluid bg-cover text-white">
      <div class="container">
        <h1 class="display-3">MENU</h1>
        <h4 class="font-weight-bolder mt-5 text-capitalize">
          Presenta tu menu de forma digital
        </h4>
      </div>
    </div>
    <Menu />
  </div>
</template>

<script>
// @ is an alias to /src
import Menu from "@/components/Menu.vue";

export default {
  name: "Home",
  components: {
    Menu
  }
};
</script>
<style scoped>
.jumbotron {
  background-image: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0.6) 0%,
      rgba(0, 0, 0, 0.6) 100%
    ),
    url("https://source.unsplash.com/GXXYkSwndP4/1600x900");
}
.bg-cover {
  background-attachment: static;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

@media (min-width: 768px) {
  .jumbotron {
    height: 50vh;
  }
}

@media (min-width: 992px) {
  .jumbotron {
    height: 60vh;
  }
}

@media (min-width: 1200px) {
  .jumbotron {
    height: 70vh;
  }
}
</style>
