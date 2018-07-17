<template>
    <div>
        <molecule-navigation-sidebar/>
    </div>
</template>

<script>
//
//
//
//
//
//

import {Vue, Component} from 'vue-property-decorator';
import MoleculeNavigationSidebar from '../../molecules/navigation/MoleculeNavigationSidebar';


@Component({
    components: {MoleculeNavigationSidebar},
})
export default class OrganismsNavigation extends Vue {
}
</script>
