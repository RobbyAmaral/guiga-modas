<template>
<div class="sidenav-container">
    <div class="sidenav-backdrop" 
        v-if="isSideNavActive"
        @click="toggle">
        <transition name="slide">
            <ul class="sidenav-panel">
                <li class="nav-item-title">
                    <span>Guiga Modas</span>
                    <p class="subtitle">Selecione um de nossos setores</p>
                </li>
                <li class="nav-item"><nuxt-link to="/feminino">Feminino</nuxt-link></li>
                <li class="nav-item"><nuxt-link to="/masculino">Masculino</nuxt-link></li>
                <li class="nav-item"><nuxt-link to="/lingerie">Lingerie</nuxt-link></li>
                <li class="nav-item"><nuxt-link to="/moda-praia">Moda Praia</nuxt-link></li>
                <li class="nav-item"><nuxt-link to="/bolsas-acessorios">Bolsas e Acessórios</nuxt-link></li>
                <transition name="typer"
                    enter-active-class="typping blink-type"
                    leave-active-class="blink-type">
                    <li class="typewriter">
                        <p>O estilo que te faz brilhar!</p>
                    </li>
                </transition>
            </ul>
        </transition>
    </div>
</div>
</template>

<script>
import { store, mutations } from '@/store/store.js'

export default {
    name: "SideNav",
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
};
</script>

<style lang="scss" scoped>
    .slide-enter-active,
    .slide-leave-active
    {
        transition: transform .5s ease-in-out;
    }

    .slide-enter,
    .slide-leave-to {
        transform: translateX(-100%);
        transition: all .5s ease-in .2s
    }

    .sidenav-backdrop {
        left: 0;
        top: 65px;
        z-index: 2;
        width: 100vw;
        height: 100vh;
        position: fixed;
        background-color: rgba(0,0,0,.5);
        transition: transform .5s ease-in-out;
    }

    .sidenav-panel {
        left: 0;
        top: 65px;
        z-index: 10;
        width: 200px;
        height: 100vh;
        position: fixed;
        overflow-y: auto;
        color: #101010;
        background-color: #ffffff;
    }
    .nav-item-title, .nav-item {
        font-size: 1.5rem;
        padding: 0.875rem;
        border-bottom: 1px solid #e9e9e9;
    }
    .nav-item-title .subtitle {
        color: #666;
        padding-top: 5px;
        font-size: .625rem;
        letter-spacing: .05rem;
    }
    .nav-item-title, .subtitle {
        text-align: center;
    }
    .nav-item a {
        font-size: 1rem;
        color: #101010;
    }
    .sidenav-panel .typewriter p {
        color: #666;
        padding-top: 1rem;
        font-size: 12px;
        text-align: center;
        overflow: hidden;
        border-right: .15em solid grey;
        white-space: nowrap;
        margin: 0 auto;
        letter-spacing: .1rem;
        animation: 
            typing 3.5s steps(40, end),
            blink-type .75s step-end infinite;
    }

@keyframes typing {
    from { width: 0 }
    to { width: 100% }
}
@keyframes blink-type {
    from, to { border-color: transparent }
    50% { border-color: grey; }
}
</style>