<template>
    <div class="image">
        <img :src="src"/>
    </div>
</template>

<script lang="ts">
import {Vue, Component, Prop} from 'vue-property-decorator';

@Component({})
export default class AtomProductImage extends Vue {
    /** イメージのURL */
    @Prop({type: String, required: true}) public src!: string;
}
</script>
