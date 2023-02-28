<script>
//import
import ComicCard from "./Comic-card.vue";

export default {
  components: { ComicCard },
  props: { comicsList: Array },
  data() {
    return {
    };
  },
};

</script>

<template>

  <main>
    <!-- place holdwer -->
    <section class="courrent-series-back">
      <div class="container flex wrap">
        <ComicCard
          v-for="comic in comicsList"
          :title="comic.series"
          :image="comic.thumb"
          :type="comic.type"
        />
        
      </div>
    </section>

    <!-- img link  -->
    <section class="link-merch-back">
      <div class="container">
        <div class="link-merch flex">

          <!-- init-col -->
          <div class="col-link flex">
            <img src="../assets/Img/buy-comics-digital-comics.png" class="img-link" alt="buy-online">
            <span class="text-link">
              DIGITAL COMICS
            </span>
          </div>
          <!-- fin-col -->

          <!-- init-col -->
          <div class="col-link flex">
            <img src="../assets/Img/buy-comics-merchandise.png" class="img-link" alt="buy-merch">
            <span class="text-link">
              DC MERCHANDISE
            </span>
          </div>
          <!-- fin-col -->

          <!-- init-col -->
          <div class="col-link flex">
            <img src="../assets/Img/buy-comics-subscriptions.png" class="img-link" alt="sub">
            <span class="text-link">
              SUBSCRIPTION
            </span>
          </div>
          <!-- fin-col -->

          <!-- init-col -->
          <div class="col-link flex">
            <img src="../assets/Img/buy-comics-shop-locator.png" class="img-link" alt="shop-map">
            <span class="text-link">
              COMIC SHOP LOCATOR
            </span>
          </div>
          <!-- fin-col -->

          <!-- init-col -->
          <div class="col-link flex">
            <img src="../assets/Img/buy-dc-power-visa.svg" class="img-link" alt="power-visa">
            <span class="text-link">
                DC POWER VISA
            </span>
          </div>
          <!-- fin-col -->

        </div>
      </div>
    </section>

  </main>

</template>

<style lang="scss" scoped>
  // current series (black part)
    
  .courrent-series-back{
    background-color: black;
  }
  //************* */

  // merch links (blue part)

  .link-merch-back{
    background-color: #0282f9;
  }

  .link-merch{
    color: white;
    gap: 1.4rem;
  }

  .img-link{
    width: 20%;
  }

  .text-link{
    padding-left: 20px;
  }

  .col-link{
    width: calc(100% / 5);
    align-items: center;
    padding: 2.5rem 0;
  }
</style>