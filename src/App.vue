<template>
    <div id="app">
        <header>
            <p>This is a header</p>
            <p>This is a header</p>
            <p>This is a header</p>
        </header>
        <nav>
            <router-link to="/">Home</router-link>
            <router-link to="/about">About</router-link>
        </nav>
        <main>
            <router-view/>
        </main>
    </div>
</template>

<style lang="scss">
    #app {
        display: grid;
        grid-template-rows: 30px calc(100vh - 50px);
        grid-template-columns: 250px 1fr;
        grid-template-areas: "header header" "nav    main";
    }

    header {
        grid-area: header;
        display: flex;
        flex-direction: row;
    }

    nav {
        grid-area: nav;
        display: flex;
        flex-direction: column;
    }

    main {
        grid-area: main;
    }

</style>
