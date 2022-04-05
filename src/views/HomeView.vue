<template>
  <div class="home">
    <CarouselComp />
    <div class="container home__offering ">
      <div class="row">
        <div class="col-md-4 home_border">
          <h3 class="home__offeringTitle">We are Offering the Best Estate Deals</h3>
        </div>
        <div class="col-md-8">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse omnis,
            nisi est labore dolorem optio ipsa culpa deleniti, ratione cumque
            minus pariatur alias tempore. Consequuntur et doloribus tempore
            corporis pariatur. Lorem ipsum dolor sit amet consectetur
            adipisicing elit. Tempore provident ullam porro dolorum rerum?
            Ducimus laborum, consequatur expedita doloremque repellat excepturi
            ipsa architecto aut ea?
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CarouselComp from "../components/CarouselComp.vue";

export default {
  name: "HomeView",
  components: {
    CarouselComp,
  },
};
</script>
