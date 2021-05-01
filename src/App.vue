<template>
    <div>
        <HelloWorld msg="Counter" />

        <div class="owner">
            <h2 class="creator">Created By:</h2>
            <p class="name"><code>.Debanjan_Tewary()</code></p>
        </div>
    </div>
</template>

<script setup>
import HelloWorld from "./components/HelloWorld.vue";

// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    /* margin-top: 10px; */
    box-sizing: border-box;
    padding: none;
    margin: 0;
    justify-content: center;
    align-items: center;
}

.logoimg {
    max-height: 30vh;
}

.owner {
    min-width: 100vw;
    max-height: 10vh;
    margin: none;
}
.owner > h2 {
    color: green;
    font-size: 20px;
    padding-bottom: 0;
    margin-bottom: 0;
}

.owner > p {
    font-size: 20px;
    font-weight: bold;
}
</style>
