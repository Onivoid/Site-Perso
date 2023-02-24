<script setup>
    definePageMeta({
        layout: "default",
    });
</script>

<template>
    <header>
        <div class="headerContainer">
            <TwtichPlayer channel="onivoid_"></TwtichPlayer>
        </div>
        <div class="favorite">

        </div>
    </header>
    <section class="favorite">
        <h1>Jeux Favorits</h1>
        <div class="favContainer">
            <div class="item">
                <img 
                    src="https://caer.univ-amu.fr/wp-content/uploads/default-placeholder.png" 
                    alt="">
                <p class="title">Titre</p>
                <p class="type">genre</p>
            </div>
            <div class="item">
                <img 
                    src="https://caer.univ-amu.fr/wp-content/uploads/default-placeholder.png" 
                    alt="">
                <p class="title">Titre</p>
                <p class="type">genre</p>
            </div>
            <div class="item">
                <img 
                    src="https://caer.univ-amu.fr/wp-content/uploads/default-placeholder.png" 
                    alt="">
                <p class="title">Titre</p>
                <p class="type">genre</p>
            </div>
            <div class="item">
                <img 
                    src="https://caer.univ-amu.fr/wp-content/uploads/default-placeholder.png" 
                    alt="">
                <p class="title">Titre</p>
                <p class="type">genre</p>
            </div>
        </div>
    </section>
</template>

<style scoped>
    @import url('../assets/css/pages/index/desktop.css');
    @import url('../assets/css/pages/index/tablet.css');
    @import url('../assets/css/pages/index/mobile.css');
    header{
    background: url('../assets/img/apexMap.jpg');
    }
</style>