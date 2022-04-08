<template>
  <div class="home">
    <carousel-comp />
    <div class="container home__offering">
      <div class="row">
        <div class="col-md-4 home_border">
          <h3 class="home__offeringTitle">
            We are Offering the Best Estate Deals
          </h3>
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
    <features-comp :data="featureData" />
    <div class="properties">
      <div class="container">
        <div class="row">
          <div class="col-md-12 col-sm-12">
            <h2 class="properties__h2">
              Featured
              <b>Properties</b>
            </h2>
          </div>
          <div class="col-md-12 col-sm-12">
            <p class="properties__subtitle">
              Quisque diam lorem interdum vitaapibus vitae pede. Donec eget
              tellus non erat lacinia fertum. Donec in velit vel ipsum
              auctovinar.
            </p>
          </div>
        </div>

        <properties-comp :propertiesData="propertiesData" />
      </div>
    </div>

    <div class="home__slider">
      <carousel-picture-content />
    </div>

    <div class="home__banner">
      <banner-comp/>
    </div>
  </div>
</template>

<script>
import { featureData, propertiesData } from "../data/data.dummy";

import CarouselComp from "../components/CarouselComp.vue";
import FeaturesComp from "../components/FeaturesComp.vue";
import PropertiesComp from "../components/PropertiesComp.vue";
import CarouselPictureContent from "../components/CarouselPictureContent.vue";
import BannerComp from "../components/BannerComp.vue";

export default {
  name: "HomeView",
  components: {
    CarouselComp,
    FeaturesComp,
    PropertiesComp,
    CarouselPictureContent,
    BannerComp,
  },
  data() {
    return {
      featureData: featureData,
      propertiesData: propertiesData,
    };
  },
};
</script>
