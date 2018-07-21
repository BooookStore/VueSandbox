<template>
    <div class="description">
        <slot/>
    </div>
</template>

<script lang="ts">
import {Vue, Component} from 'vue-property-decorator';

@Component({})
export default class AtomDescription extends Vue {

}
</script>

<style scoped>

</style>