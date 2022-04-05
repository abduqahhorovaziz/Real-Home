<template>
<div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
  <ol class="carousel-indicators home__carousel-indicators">
    <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
    <li data-target="#carouselExampleCaptions" data-slide-to="1"></li>
    <li data-target="#carouselExampleCaptions" data-slide-to="2"></li>
  </ol>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="../assets/images/slide.png" class="d-block w-100" alt="">
      <div class="carousel-caption d-none d-md-block">
        <h5>120 Anastasia Avenue, Coral Gables</h5>
        <p>$625,000</p>
        <button type="button" class="btn btn-outline-light">MORE INFO</button>
      </div>
    </div>
    <div class="carousel-item">
      <img src="../assets/images/slide.png" class="d-block w-100" alt="">
      <div class="carousel-caption d-none d-md-block">
        <h5>Second slide label</h5>
        <p>Some representative placeholder content for the second slide.</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="../assets/images/slide.png" class="d-block w-100" alt="">
      <div class="carousel-caption d-none d-md-block">
        <h5>Third slide label</h5>
        <p>Some representative placeholder content for the third slide.</p>
      </div>
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-target="#carouselExampleCaptions" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-target="#carouselExampleCaptions" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </button>
</div>
</template>

<style lang="scss">
.home{
  &__carousel-indicators{
    bottom: 200px;
  }
}

</style>