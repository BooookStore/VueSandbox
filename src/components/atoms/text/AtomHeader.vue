<template>
    <div class="header">
        <slot/>
    </div>
</template>

<script lang="ts">
import {Vue, Component} from 'vue-property-decorator';

@Component({})
export default class AtomHeader extends Vue {
    // todo : heading level can specifiable.
}
</script>
