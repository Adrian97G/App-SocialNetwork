<template>
    <footer class="mt-5">
        <ul class="list-group list-group-flush list-group-horizontal text-center mb-0">
            <li class="list-group-item">
                <router-link class="router-link" to="/">Home</router-link>
            </li>
            <li class="list-group-item">
                <router-link class="router-link" to="/about">About</router-link>
            </li>
            <li class="list-group-item">
                <router-link class="router-link" to="/posts">Posts</router-link>
            </li>
        </ul>
        <img src="letra d.png" alt="Logo">
        <div class="text-black-50 text-center">devbook &#169; 2023</div>
    </footer>
</template>

<style scoped>
    footer {
        width: 100%;
    }
    img {
        width: 20px;
        margin: 0 auto;
        display: block;
    }
    .list-group {
        justify-content: center;
    }
    .list-group-item {
        border: none;
    }
    .router-link {
        text-decoration: none;
    }
</style>