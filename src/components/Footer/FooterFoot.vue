<template>
  <footer class="footer footer_bg">
    <div class="container">
      <div class="row">
        <FooterIcons />
        <FooterNavigation :footerMenu="footerMenu" />
        <FooterClient :footerClient="footerClient" />
        <FooterContacts/>
      </div>
    </div>
  </footer>
</template>

<script>
import { menuList, menuClient } from "../../constants/menuLinks.js";

import FooterIcons from "./FooterIcons.vue";
import FooterNavigation from "./FooterNavigation.vue";
import FooterClient from "./FooterClient.vue";
import FooterContacts from "./FooterContacts.vue";

export default {
  data() {
    return {
      footerMenu: menuList,
      footerClient: menuClient,
    };
  },
  components: {
    FooterIcons,
    FooterNavigation,
    FooterClient,
    FooterContacts,
  },
};
</script>