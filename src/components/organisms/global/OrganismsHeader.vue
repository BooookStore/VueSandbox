<template>
    <div class="ui attached stackable borderless menu">
        <molecule-logo-link class="item"/>
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
