<template>
  <main>
    <div class="banner goodspage-banner">
      <div class="container">
        <div class="row">
          <div class="col-lg-6">
            <nav-bar-component />
          </div>
        </div>
        <h1 class="title-big">For your pleasure</h1>
      </div>
    </div>
    <section class="shop">
      <div class="container">
        <div class="row">
          <div class="col-lg-4 offset-2">
            <img
              class="shop__girl"
              src="@/assets/img/coffee_goods.jpg"
              alt="girl"
            />
          </div>
          <div class="col-lg-4">
            <div class="title">About our beans</div>
            <img
              class="beanslogo"
              src="@/assets/logo/Beans_logo_dark.svg"
              alt="Beans logo"
            />
            <div class="shop__text">
              Extremity sweetness difficult behaviour he of. On disposal of as
              landlord horrible.
              <br /><br />
              Afraid at highly months do things on at. Situation recommend
              objection do intention<br />
              so questions. <br />
              As greatly removed calling pleased improve an. Last ask him cold
              feel<br />
              met spot shy want. Children me laughing we prospect answered
              followed. At it went<br />
              is song that held help face.
            </div>
          </div>
        </div>

        <div class="line"></div>

        <div class="row">
          <div class="col-lg-10 offset-lg-1">
            <div class="shop__wrapper">
              <div class="best__item">
                <img
                  :src="require(`@/assets/img/${cards[0].path}`)"
                  :alt="cards[0].path"
                />
                <div class="best__item-title">{{ cards[0].text }}</div>
                <div class="best__item-price">{{ cards[0].price }}</div>
              </div>

              <div class="best__item">
                <img
                  :src="require(`@/assets/img/${cards[1].path}`)"
                  :alt="cards[0].path"
                />
                <div class="best__item-title">{{ cards[1].text }}</div>
                <div class="best__item-price">{{ cards[1].price }}</div>
              </div>

              <div class="best__item">
                <img
                  :src="require(`@/assets/img/${cards[2].path}`)"
                  :alt="cards[0].path"
                />
                <div class="best__item-title">{{ cards[2].text }}</div>
                <div class="best__item-price">{{ cards[2].price }}</div>
              </div>

              <div class="best__item">
                <img
                  :src="require(`@/assets/img/${cards[3].path}`)"
                  :alt="cards[0].path"
                />
                <div class="best__item-title">{{ cards[3].text }}</div>
                <div class="best__item-price">{{ cards[3].price }}</div>
              </div>

              <div class="best__item">
                <img
                  :src="require(`@/assets/img/${cards[4].path}`)"
                  :alt="cards[0].path"
                />
                <div class="best__item-title">{{ cards[4].text }}</div>
                <div class="best__item-price">{{ cards[4].price }}</div>
              </div>

              <div class="best__item">
                <img
                  :src="require(`@/assets/img/${cards[5].path}`)"
                  :alt="cards[0].path"
                />
                <div class="best__item-title">{{ cards[5].text }}</div>
                <div class="best__item-price">{{ cards[5].price }}</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import NavBarComponent from "@/components/NavBarComponent.vue";
import CardComponent from "@/components/CardComponent.vue";
export default {
  components: { NavBarComponent, CardComponent },
  data() {
    return {
      cards: [
        {
          id: 0,
          path: "coffee-1.jpg",
          text: "Solimo Coffee Beans 2kg",
          price: "10.73$",
        },
        {
          id: 1,
          path: "coffee-1.jpg",
          text: "Solimo Coffee Beans 2kg",
          price: "10.73$",
        },
        {
          id: 2,
          path: "coffee-1.jpg",
          text: "Solimo Coffee Beans 2kg",
          price: "10.73$",
        },
        {
          id: 3,
          path: "coffee-1.jpg",
          text: "Solimo Coffee Beans 2kg",
          price: "10.73$",
        },
        {
          id: 4,
          path: "coffee-1.jpg",
          text: "Solimo Coffee Beans 2kg",
          price: "10.73$",
        },
        {
          id: 5,
          path: "coffee-1.jpg",
          text: "Solimo Coffee Beans 2kg",
          price: "10.73$",
        },
      ],
    };
  },
};
</script>
