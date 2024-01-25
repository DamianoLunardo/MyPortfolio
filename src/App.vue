<script>
import AppHeader from './components/AppHeader.vue';
import ChiSono from './components/ChiSono.vue';

export default {
    components: {
        AppHeader,
        ChiSono,
    }
}

</script>

<template>
    <AppHeader />
    <ChiSono />
</template>

<style lang = "scss">
@use "./styles/general.scss" as *;


</style>
