<template>
  <div class="properties">
    <div class="container">
      <div class="row d-flex justify-content-between">
        <div
          class="col-md-4 col-sm-12"
          v-for="property in propertiesData"
          :key="property.id"
        >
          <div class="properties__col">
            <img
              :src="require(`../assets/images/${property.image}.png`)"
              :alt="property.desc.sqft"
              class="properties__img"
            />
            <h4 class="properties__h4">
              {{ `${property.desc.sqft} ${property.title}` }}
            </h4>
            <p class="properties__sub">{{ property.subtitle }}</p>
            <p class="properties__price">${{ property.price.toFixed(3) }}</p>
            <ul class="properties__desc">
              <li class="properties__item">{{ property.desc.sqft }} Sq Ft</li>
              <li class="properties__item">
                {{ property.desc.rooms }} Bedrooms
              </li>
              <li class="properties__item">
                {{ property.desc.bath }} Bathrooms
              </li>
            </ul>
          </div>
         
        </div>
         <div class="col">
            <button type="button" class="btn btn-primary properties__more">All properties</button>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    propertiesData: {
      type: Array,
      default: () => [],
    },
  },
};
</script>