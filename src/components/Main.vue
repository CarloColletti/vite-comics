<script>

</script>

<template>

  <main>
    <!-- place holdwer -->
    <section class="place-holder-back">
      <div class="container">
        <div class="content">
          <span class="place-holder">
            --> Content goes here
          </span>
        </div>
      </div>
    </section>

    <!-- img link  -->
    <section class="link-merch-back">
      <div class="container">
        <div class="link-merch flex">

          <!-- init-col -->
          <div class="col flex">
            <img src="../assets/Img/buy-comics-digital-comics.png" class="img-link" alt="buy-online">
            <span class="text-link">
              DIGITAL COMICS
            </span>
          </div>
          <!-- fin-col -->

          <!-- init-col -->
          <div class="col flex">
            <img src="../assets/Img/buy-comics-merchandise.png" class="img-link" alt="buy-merch">
            <span class="text-link">
              DC MERCHANDISE
            </span>
          </div>
          <!-- fin-col -->

          <!-- init-col -->
          <div class="col flex">
            <img src="../assets/Img/buy-comics-subscriptions.png" class="img-link" alt="sub">
            <span class="text-link">
              SUBSCRIPTION
            </span>
          </div>
          <!-- fin-col -->

          <!-- init-col -->
          <div class="col flex">
            <img src="../assets/Img/buy-comics-shop-locator.png" class="img-link" alt="shop-map">
            <span class="text-link">
              COMIC SHOP LOCATOR
            </span>
          </div>
          <!-- fin-col -->

          <!-- init-col -->
          <div class="col flex">
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
  // debug 
  .place-holder{
    color: white;
    font-size: 1.4rem;
  }
  
  .content{
    height: 120px;
  }
  
  .place-holder-back{
    background-color: black;
  }
  //************* */

  .link-merch-back{
    background-color: #0282f9;
  }

  .link-merch{
    color: white;
    gap: 1.4rem;
  }

  .img-link{
    width: 25%;
  }

  .text-link{
    padding-left: 20px;
  }

  .col{
    width: calc(100% / 5);
    align-items: center;
    padding: 2.5rem 0;
  }
</style>