<template>
  <div class="menu container">
    <div class="row">
      <div
        v-for="item in menuItems"
        :key="item.id"
        class="col-12 col-sm-12 col-md-6"
      >
        <div class="card-deck">
          <div class="card mb-3 bg-light">
            <div class="media">
              <img
                :src="item.image"
                class="align-self-center mr-3 menu-thumbnail img-thumbnail"
                :alt="item.title"
              />
              <div class="media-body">
                <h5 class="mt-3">
                  <u>{{ item.title }}</u>
                </h5>
                <p class="text-left">
                  Cras sit amet nibh libero, in gravida nulla. Nulla vel metus
                  |<small class="text-muted"> Lps. 100</small>
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data: function() {
    return {
      menuItems: [
        {
          id: 1,
          title: "Cerdo Glaceado",
          image: require("../assets/image-1.jpg")
        },
        {
          id: 2,
          title: "Pasta Fresca",
          image: require("../assets/image-2.jpg")
        },
        { id: 3, title: "Burritos", image: require("../assets/image-3.jpg") },
        { id: 4, title: "Panqueques", image: require("../assets/image-4.jpg") }
      ]
    };
  }
};
</script>
<style scoped>
.menu-thumbnail {
  width: 8em;
  height: 8em;
}

img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}
</style>
