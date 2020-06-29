<template>
  <section class="header-container">
      <div class="header">
          <SideNavToggle />
          <div class="logo">
            <nuxt-link to="/"><img src="~assets/images/guiga-logo.png" alt="Guiga Modas logo" width=110 height=55></nuxt-link>
            <p class="subtitle">GUIGA MODAS</p>
          </div>
      </div>
      <SideNav />
      <div class="navigation-items">
          <ul class="nav-list">
              <li class="nav-item"><nuxt-link to="/feminino">Feminino</nuxt-link></li>
              <li class="nav-item"><nuxt-link to="/masculino">Masculino</nuxt-link></li>
              <li class="nav-item"><nuxt-link to="/lingerie">Lingerie</nuxt-link></li>
              <li class="nav-item"><nuxt-link to="/moda-praia">Moda Praia</nuxt-link></li>
              <li class="nav-item"><nuxt-link to="/bolsas-acessorios">Bolsas e Acessórios</nuxt-link></li>
          </ul>
      </div>
  </section>
</template>

<script>
import SideNavToggle from "@/components/Navigator/SideNavToggle";
import SideNav from "@/components/Navigator/SideNav"

export default {
  name: "Header",
  components: {
    SideNavToggle,
    SideNav
  }
};
</script>

<style lang="scss">
.header-container {
    width: 100%;
    // position: fixed;
}

.header {
  height: 100px;
  border-image-slice: 1;
  box-sizing: border-box;
  background-color: black;
  border-bottom: 3px solid white;
  border-image-source: linear-gradient(to right, #D3D3D3, black);
  .icon-menu {
    display: none;
  }
  .logo, .subtitle {
    top: 10%;
    width: 150px;
    margin: 0 auto;
    text-align: center;
    position: relative;
  }
  .subtitle {
    color: white;
    font-size: 20px;
    font-weight: 700;
    letter-spacing: 1px;
  }
}

.navigation-items {
    display: block;
    height: 42px;
    background-color: white;
    border-bottom: 1px solid black;
    .nav-list {
      margin: 0;
      display: flex;
      color: inherit; 
      font-size: 18px;
      padding-top: 9px;
      justify-content: center; 
      .nav-item a { 
        color: #666;
        padding-right: 20px;
        text-decoration: none;
      }
    }
}

@media (max-width: 525px) {
  .header {
    height: 65px;
    .subtitle {
      display: none;
    }
    .icon-menu .bar {
      width: 90%;
      height: 2px;
      float: left;
      background-color: white;
    }
    .logo img {
      width: 90px;
      height: 50px;
    }
  }
  .navigation-items {
    display: none;
  }
}
</style>
