<template>
    <span>
        <v-navigation-drawer app v-model="drawer">
            <v-list>
                <template v-for="(menu, i) in menus">
                    <v-list-tile :key="i">
                        <v-list-tile-content>
                            {{menu.value}}
                        </v-list-tile-content>
                    </v-list-tile>
                    <v-divider :key="`divider-${i}`"></v-divider>
                </template>
            </v-list>
        </v-navigation-drawer>
        <v-toolbar app dark>
            <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-toolbar-side-icon>
            <v-spacer class="hidden-md-and-up"></v-spacer>
            <v-img src="https://assets.logrocket.io/img/logo.png" max-width="120px" max-height="25px"></v-img>
            <v-btn flat class="hidden-sm-and-down">Timelapse</v-btn>
            <v-spacer class="hidden-sm-and-down"></v-spacer>
            <v-btn flat class="hidden-sm-and-down">Skills</v-btn>
            <v-btn flat class="hidden-sm-and-down">Projects</v-btn>
            <v-btn flat class="hidden-sm-and-down">Links</v-btn>
        </v-toolbar>
    </span>
</template>

<script>
export default {
    name: 'RocketNavigation',
    data() {
        return {
            drawer: false,
            menus: [
                { value: 'Timelapse' },
                { value: 'Skills' },
                { value: 'Projects' },
                { value: 'Links' }
            ]
        };
    }
};
</script>

<style scoped>
</style>