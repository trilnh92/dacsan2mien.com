<template>
  <section class="under-construction">
    <div class="under-construction__content">
      <h3>
        COMING SOON
      </h3>
      <p>Make dacsan2mien great again.</p>
    </div>
    <img :src="require('../assets/bg01.jpg')"/>
  </section>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component
export default class UnderConstruction extends Vue {

}
</script>

<style scoped lang="scss">
  h3 {
    font-family: 'Playfair Display', serif;
    font-size: 60px;
    font-weight: 500;
    color: #333;
    line-height: 1.1;
    text-transform: uppercase;
  }

  p {
    font-family: 'Poppins', sans-serif;
    font-size: 24px;
    color: #999;
    line-height: 1.2;
    font-weight: 400;
  }

  .under-construction {
    display: grid;
    grid-template-columns: 37% 63%;
    grid-template-rows: 1fr;
    grid-template-areas: ". .";
    align-items: center;
    height: 100vh;
    width: 100%;

    &__background {

    }
  }

  img {
    object-fit: fill;
    width: 100%;
    height: 100%;
  }
</style>
