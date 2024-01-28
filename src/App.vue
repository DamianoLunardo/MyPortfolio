<script>
import AppHeader from './components/AppHeader.vue';
import ChiSono from './components/ChiSono.vue';
import AboutMe from './components/About.vue';

export default {
    components: {
        AppHeader,
        ChiSono,
        AboutMe,
    }
}

</script>

<template>
    <AppHeader />
    <ChiSono />
    <AboutMe />
</template>

<style lang = "scss">
@use "./styles/general.scss" as *;


</style>
