<template>
    <div class="meta">
        <slot/>
    </div>
</template>

<script lang="ts">
import {Vue, Component} from 'vue-property-decorator';

@Component({})
export default class AtomMeta extends Vue {

}
</script>

<style scoped>

</style>