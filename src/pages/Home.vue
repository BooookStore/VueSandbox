<template>
    <div>
        <molecule-product-card
                :imageUrl="sampleImage"
                name="Vue"
                category="JavaScript"
                description="high usability framework"/>
    </div>
</template>

<script lang="ts">
import {Component, Vue} from 'vue-property-decorator';
import AtomProductImage from '../components/atoms/image/AtomProductImage';
import AtomHeader from '../components/atoms/text/AtomHeader';

// noinspection TypeScriptCheckImport
import sampleImage from '@/assets/logo.png';
import MoleculeProductCard from '../components/molecules/card/MoleculeProductCard';

@Component({
    components: {
        MoleculeProductCard,
        AtomHeader,
        AtomProductImage,
    },
})
export default class Home extends Vue {
    private sampleImage: string = sampleImage;
}
</script>
