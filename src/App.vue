<script>
import AppHeader from './components/AppHeader.vue';
import ChiSono from './components/ChiSono.vue';
import AboutMe from './components/About.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contacts.vue';
import Footer from './components/Footer.vue';

export default {
    components: {
        AppHeader,
        ChiSono,
        AboutMe,
        Projects,
        Contact,
        Footer,
    }
}

</script>

<template>
    <AppHeader />
    <ChiSono />
    <AboutMe />
    <Projects />
    <Contact />
    <Footer />
</template>

<style lang = "scss">
@use "./styles/general.scss" as *;


</style>
