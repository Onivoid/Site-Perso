<script setup>
    import {ref} from 'vue';

    let isActive = ref(false);

    const mobileButtonHandler = (e) => {
        isActive.value = !isActive.value;
    }
</script>
<template>
    <main>
        <div class="navigation">
            <div class="mobileNavButton">
                <i  class="fas" 
                    :class="{'fa-bars': !isActive, 'fa-xmark': isActive}" 
                    @click="mobileButtonHandler">
                </i>
            </div>
            <div class="left">
                <NuxtLink to="#">
                    <img src="../assets/img/logo.png" alt="Onivoid Logo">
                </NuxtLink>
            </div>
            <nav class="middle">
                <ul>
                    <li>
                        <NuxtLink to="#">Accueil</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="#">Réseaux</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="#">Portfolio</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="#">Shop</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="#">Contact</NuxtLink>
                    </li>
                </ul>
            </nav>
            <div class="right">
                <NuxtLink to="#">
                    <img src="../assets/img/discord_logo.png" alt="Discord Logo">
                    <span>
                        <p class="small">Rejoins</p>
                        <p class="big">La Taverne</p>
                    </span>
                </NuxtLink>
            </div>
        </div>
        <div class="mobileNavContainer" :class="{'isActive': isActive}">
            <ul>
                <li>
                    <NuxtLink to="#" @click="mobileButtonHandler">Accueil</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="#" @click="mobileButtonHandler">Réseaux</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="#" @click="mobileButtonHandler">Portfolio</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="#" @click="mobileButtonHandler">Shop</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="#" @click="mobileButtonHandler">Contact</NuxtLink>
                </li>
            </ul>
        </div>
      <slot />
    </main>
</template>

<style scoped>
    @import url('../assets/css/layouts/default_global.css');
    @import url('../assets/css/layouts/default_desktop.css');
    @import url('../assets/css/layouts/default_tablet.css');
    @import url('../assets/css/layouts/default_mobile.css');
</style>