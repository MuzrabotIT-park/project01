<template>
  <button class="site_btn">
    <slot />
  </button>
</template>

<script>
export default {};
</script>

<style lang="scss" >
@import "../../assets/styles/components/_vars.scss";
@import "../../assets/styles/components/_mixsin.scss";

.site_btn {
  font-size: 17px;
  padding: 0.5em 2em;
  border: transparent;
  background: linear-gradient(
      90deg,
      rgb(14, 165, 234),
      rgb(11, 209, 209) 51%,
      rgb(14, 165, 234)
    )
    var(--x, 0) / 200%;
  color: #ffffff;
  transition: 0.5s;
  cursor: pointer;
}

.site_btn:hover {
    background: linear-gradient(
      90deg,
      rgb(14, 165, 234),
      rgb(11, 209, 209) 51%,
      rgb(14, 165, 234)
    )
    var(--x, 0) / 80%;
}

.site_btn:active {
  transform: translate(0em, 0.2em);
}
</style>