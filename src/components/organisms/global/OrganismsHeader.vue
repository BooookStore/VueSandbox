<template>
    <div id="root">
        <molecule-logo-link/>
    </div>
</template>

<script lang="ts">
    import {Component, Vue} from 'vue-property-decorator';

    import MoleculeLogoLink from '@/components/molecules/media/MoleculeLogoLink';

    @Component({
        components: {MoleculeLogoLink},
    })
    export default class OrganismsHeader extends Vue {
    }
</script>

<style scoped lang="scss">
    #root {
        background-color: #ff9200;
    }
</style>