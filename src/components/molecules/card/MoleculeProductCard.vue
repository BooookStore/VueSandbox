<template>
    <div class="ui card">
        <atom-product-image :src="imageUrl"/>
        <div class="content">
            <atom-header>{{name}}</atom-header>
            <atom-meta>{{category}}</atom-meta>
            <atom-description>{{description}}</atom-description>
        </div>
    </div>
</template>

<script lang="ts">
import {Vue, Component, Prop} from 'vue-property-decorator';
import AtomProductImage from '../../atoms/image/AtomProductImage';
import AtomHeader from '../../atoms/text/AtomHeader';
import AtomDescription from '../../atoms/text/AtomDescription';
import AtomMeta from '../../atoms/text/AtomMeta';

@Component({
    components: {AtomMeta, AtomDescription, AtomHeader, AtomProductImage},
})
export default class MoleculeProductCard extends Vue {

    @Prop({type: String, required: true}) public imageUrl: string;

    @Prop({type: String, required: true}) public name: string;

    @Prop({type: String, required: true}) public category: string;

    @Prop({type: String, required: true}) public description: string;

}
</script>

<style scoped>

</style>