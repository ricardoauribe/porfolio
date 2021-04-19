<template>
    <v-app>
        <rocket-navigation></rocket-navigation>
        <rocket-plans></rocket-plans>
        <rocket-footer></rocket-footer>
    </v-app>
</template>

<script>
import RocketNavigation from '@/components/Navigation';
import RocketPlans from '@/components/Plans';
import RocketFooter from '@/components/Footer';
export default {
    name: 'LogRocketApp',
    components: {
        RocketNavigation,
        RocketPlans,
        RocketFooter
    }
};
</script>

<style>
</style>