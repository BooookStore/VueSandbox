<template>
    <div class="ui inverted vertical menu">
        <router-link class="item" to="/">Home</router-link>
        <router-link class="item" to="/about">About</router-link>
    </div>
</template>

<script lang="ts">
import {Vue, Component} from 'vue-property-decorator';

@Component({})
export default class MoleculeSidebarNavigation extends Vue {
}
</script>

