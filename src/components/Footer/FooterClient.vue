<template>
  <div class="col">
    <h3 class="footer__title">For clients</h3>
    <ul class="footer__list footer__list_capitalize">
      <li v-for="({ name, path }, i) in footerClient" :key="i">
        <router-link :to="path" class="footer__link">
          {{ name }}
        </router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
    props: {
        footerClient: {
            type: Array,
            required: true
        }
    }
}
</script>