<template>
    <div id="app">
        <header>
            <organisms-header/>
        </header>
        <nav>
            <organisms-navigation/>
        </nav>
        <main>
            <router-view/>
        </main>
    </div>
</template>

<!--suppress TypeScriptCheckImport -->
<script lang="ts">
import {Component, Vue} from 'vue-property-decorator';

import OrganismsHeader from '@/components/organisms/global/OrganismsHeader';
import OrganismsNavigation from '@/components/organisms/global/OrganismsNavigation';

@Component({
    components: {OrganismsNavigation, OrganismsHeader},
})
export default class App extends Vue {

}
</script>

<style lang="scss">
    #app {
        display: grid;
        grid-template-rows: 50px calc(100vh - 50px);
        grid-template-columns: max-content 1fr;
        grid-template-areas: "header header" "nav    main";
    }

    header {
        grid-area: header;
        display: flex;
        flex-direction: row;
    }

    nav {
        grid-area: nav;
        display: flex;
        flex-direction: column;
    }

    main {
        grid-area: main;
        padding: 10px;
    }

</style>
