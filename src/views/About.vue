<template>
  <div class="about">
    <header>
      <nav class="burger">
      <transition
      name="fade"
      mode="out-in">
        <hamburger-icon />
      </transition>
      </nav>
    </header>
    <h1>Vårt Kaffe</h1>
    <p
      class="thickboi"
    >Pumpkin spice mug, barista cup, sit macchiato, kopi-luwak, doppio, grounds dripper, crema, strong whipped, variety extra iced id lungo half and half mazagran. Pumpkin spice.</p>
    <p>Que dark fair trade, spoon decaffeinated, barista wings whipped, as rich aftertaste, con panna milk black, arabica white rich beans single shot extra affogato. So affogato macchiato sit extraction instant grinder seasonal organic, turkish single shot, single origin, and robusta strong to go so dripper. Viennese froth, grounds caramelization skinny aromatic cup kopi-luwak, fair trade flavour, frappuccino medium, café au lait flavour cultivar ut bar instant kopi-luwak.</p>
    <p>Roast id macchiato, single shot siphon mazagran milk fair trade est aroma a half and half and, so, galão iced to go, whipped as cream cup pumpkin spice iced. At extra, rich grinder, brewed to go, steamed half and half at, that, percolator macchiato trifecta and body as arabica dripper. In galão black java milk sit trifecta, robusta, acerbic café au lait instant shop latte. Seasonal bar shop filter aroma id, crema, affogato viennese cultivar aftertaste, seasonal, percolator cream black, galão flavour, milk aromatic turkish skinny crema.</p>
    <section class="aboutFooter">
      <img class="eva" src="./../assets/graphics/eva-cortado.jpg" alt="Eva Cortado" />
      <h2>Eva Cortado</h2>
      <p class="proff">Big Tings and That</p>
    </section>
    <footer />
  </div>
</template>
<script>
import HamburgerIcon from "../components/HamburgerIcon";
export default {
  name: "Home",
  components: {
    "hamburger-icon": HamburgerIcon
  }
};
</script>
<style lang="scss" scoped>
.about {
  h1 {
    margin: 0 auto;
  }

  .aboutFooter {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  footer {
    margin-top: 0;
  }

  .eva {
    width: 7rem;
    height: 7rem;
    border-radius: 999rem;
    margin: 1rem;
  }
  h2 {
    font-size: 1.4rem;
    margin: 0;
    padding: 0;
  }
  .thickboi {
    font-weight: 600;
    font-size: 1rem;
    margin: 0;
    line-height: 140%;
  }
  .proff {
    margin-bottom: 4rem;
    padding: 0;
    font-size: 1rem;
  }
}

//animation

.fade-enter-active,
.fade-leave-active {
  transition-duration: 0.3s;
  transition-property: height, opacity;
  transition-timing-function: ease;
  overflow: hidden;
}

.fade-enter,
.fade-leave-active {
  opacity: 0
}
</style>