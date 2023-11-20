<template>
  <section class="navbar" @actionBody="$emit('actionBody')">
    <!--  -->
    <div class="logo">
      <img :src="logoImage" alt="" />
    </div>
    <!--  -->
    <ul class="menu">
      <li v-for="(item, index) in menuArray" :key="index">
        <a :href="item.ctg_name.link">{{ item.ctg_name.text }}</a>
        <i class="fa-solid fa-play fa-rotate-90"></i>
      </li>
    </ul>
    <!--  -->
    <div class="menu_box">
      <div class="navbar_search">
        <i class="fas fa-search"></i>
      </div>
      <!--  -->
      <div class="dark_Ligth">
        <nav-dark-light />
      </div>
      <!--  -->
      <div class="navbar_btn">
        <site_btnVue>Subscribe</site_btnVue>
      </div>
    </div>
  </section>
</template>

<script>
import navDarkLight from "./component/navDarkLight.vue";
import site_btnVue from "./component/site_btn.vue";
export default {
  components: { navDarkLight, site_btnVue },
  data() {
    return {
      logoImage: require("../assets/images/Home/logo/logo.png"),
      menuArray: [
        {
          ctg_name: {
            text: "Home",
            link: "",
          },
          menu_hover: {
            page: {
              text: "Homepage-1",
              link: "",
            },
            page: {
              text: "Homepage-2",
              link: "",
            },
            page: {
              text: "Homepage-3",
              link: "",
            },
            page: {
              text: "Homepage-4",
              link: "",
            },
          },
        },
        {
          ctg_name: {
            text: "About ME",
            link: "",
          },
          menu_hover: {
            page: {
              text: "Homepage-1",
              link: "",
            },
            page: {
              text: "Homepage-2",
              link: "",
            },
            page: {
              text: "Homepage-3",
              link: "",
            },
            page: {
              text: "Homepage-4",
              link: "",
            },
          },
        },
        {
          ctg_name: {
            text: "Category",
            link: "",
          },
          menu_hover: {
            page: {
              text: "Homepage-1",
              link: "",
            },
            page: {
              text: "Homepage-2",
              link: "",
            },
            page: {
              text: "Homepage-3",
              link: "",
            },
            page: {
              text: "Homepage-4",
              link: "",
            },
          },
        },
        {
          ctg_name: {
            text: "Single Post",
            link: "",
          },
          menu_hover: {
            page: {
              text: "Homepage-1",
              link: "",
            },
            page: {
              text: "Homepage-2",
              link: "",
            },
            page: {
              text: "Homepage-3",
              link: "",
            },
            page: {
              text: "Homepage-4",
              link: "",
            },
          },
        },
        {
          ctg_name: {
            text: "Pages",
            link: "",
          },
          menu_hover: {
            page: {
              text: "Homepage-1",
              link: "",
            },
            page: {
              text: "Homepage-2",
              link: "",
            },
            page: {
              text: "Homepage-3",
              link: "",
            },
            page: {
              text: "Homepage-4",
              link: "",
            },
          },
        },
        {
          ctg_name: {
            text: "Contact",
            link: "",
          },
        },
      ],
    };
  },
};
</script>

<style lang="scss" >
@import "../assets/styles/layout/navbar.scss";
</style>