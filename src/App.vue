<template>
    <v-app>
        <rocket-navigation></rocket-navigation>
        <rocket-plans></rocket-plans>
        <footer></footer>
    </v-app>
</template>

<script>
import RocketNavigation from '@/components/Navigation';
import RocketPlans from '@/components/Plans';
import Footer from '@/components/Footer';
export default {
    name: 'LogRocketApp',
    components: {
        RocketNavigation,
        RocketPlans,
        Footer
    }
};
</script>

<style>
</style>