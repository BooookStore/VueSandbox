<template>
    <img :src="src"/>
</template>

<script lang="ts">
import {Vue, Component, Prop} from 'vue-property-decorator';

@Component({})
export default class AtomProductImage extends Vue {
    /** イメージのURL */
    @Prop(String) public src: string;
}
</script>
