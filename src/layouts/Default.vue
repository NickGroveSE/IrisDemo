<script setup>

</script>

<template>

    <header>
        <div class="header-element" id="app-name">
            Iris
        </div>
        <a class="header-element" id="app-logo">
            Logo
        </a>
    </header>

    <main id="main">
        <slot/>
    </main>

    <footer>
        <a class="footer-element" href="https://nickgrove.netlify.app/">My Portfolio Site</a>
        <a class="footer-element" href="https://github.com/NickGroveSE">Github</a>
        <a class="footer-element" >Buy Me a Coffee :)</a>
    </footer>

</template>

<style scoped>

    /* Header Styling */
    header {
        height: 60px;
    }

    .header-element {
        vertical-align: top;
        margin: 10px 10px 10px 0;
        line-height: 40px;
        display: inline-block;
    }

    #app-name {
        font-size: 20px;
    }

    #app-logo {
        width: 60px;
        height: 40px;
        border-radius: 20px;
        background-color: var(--primary-accent);
        text-align: center;
    }

    /* Main Styling */
    #main {
        width: 100%;
        height: calc(100vh - 120px);
    }

    /* Footer Styling */
    footer {
        height: 60px;
        width: 100%;
        margin: auto 0;
        text-align: center;
    }

    .footer-element {
        vertical-align: top;
        margin: 10px 10px 10px 10px;
        line-height: 40px;
        display: inline-block;
        color: var(--text);
        
    }

</style>

<!-- <script setup>
</script>

<template>



</template>

<style scoped>
</style> -->