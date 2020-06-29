<template>
    <div class="menu-icon"
        role="button" 
        :class="{ 'active' : isSideNavActive }"
        @click.prevent="toggle">
        <div class="bar bar--1"></div>
        <div class="bar bar--2"></div>
        <div class="bar bar--3"></div>
        <span class="menu-title">Menu</span>
    </div>
</template>

<script>
import { store, mutations } from '@/store/store.js'

export default {
    name: "SideNavToggle",
    computed: {
        isSideNavActive() { 
            return store.isNavOpen
        }
    },
    methods: {
        toggle() {
            mutations.toggleNav();
        }
    }
}
</script>

<style lang="scss" scoped>
  .menu-icon {
      display: none;
  }

@media (max-width: 525px) {
    .menu-icon {
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        height: 45%;
        width: 30px;
        float: left;
        position: relative;
        top: 30%;
        padding-left: 15px;
        .bar {
            width: 75%;
            height: 3px;
            background-color: white;
        }
        .menu-title {
            color: white;
            position: absolute;
            padding-left: 28px;
        }
    }
}
</style>
