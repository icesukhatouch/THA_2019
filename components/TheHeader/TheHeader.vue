<template>
    <header class="main-header">
        <nav class="main-nav">
            <ul class="nav-links">
                <div class="vertical-line-head"></div>
                <nuxt-link to="/" tag="li"><a>TICKET</a></nuxt-link>
                <div class="vertical-line"></div>
                <nuxt-link to="/" tag="li"><a>NEWS</a></nuxt-link>
                <div class="vertical-line"></div>
                <nuxt-link to="/" tag="li"><a>AGENDA</a></nuxt-link>
                <div class="vertical-line"></div>
                <nuxt-link to="/en" tag="li"><a>ENGLISH</a></nuxt-link>
                <div class="vertical-line-head"></div>
            </ul>
        </nav>
    </header>
</template>

<style scoped>
    .main-header {
        position: fixed;
        left: 2rem;
        display: flex;
        flex-direction: column;
        font-size: 2rem;
        height: 100%
    }
    .main-nav {
        height: 100%;
    }
    .nav-links {
        height: 100%;
        list-style: none;
        margin: 0;
        padding: 0;
        text-align: center;
    }
    .nav-links a {
        text-decoration: none;
        color: white;
    }
    .vertical-line {
        border-right: 1px solid white;
        width: 50%;
        height: 4rem;
    }
    .vertical-line-head {
        border-right: 1px solid white;
        width: 50%;
        height: 25%;
    }
</style>

