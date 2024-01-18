
<!-- 

Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone.

 -->

<script>
import AppHeader from './components/AppHeader.vue';
import AppContent from './components/AppContent.vue';
import AppMain from './components/AppMain.vue';
import AppFooterTop from './components/AppFooterTop.vue';
import AppFooterBottom from './components/AppFooterBottom.vue';



export default {
    data() {
        return {

        };
    },
    components: {
        AppHeader,
        AppMain,
        AppContent,
        AppFooterTop,
        AppFooterBottom,

    },  
    methods: {

    }
}
</script>

<template>

    <AppHeader />

    <AppContent />

    <AppMain />

    <AppFooterTop />

    <AppFooterBottom />

</template>

<style lang="scss">
@use "assets/scss/main" as *;
@import "assets/scss/partials/reset";
</style>
