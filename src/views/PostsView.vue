<template>
    <div class="posts">
    <img src="../assets/img/devbook.svg" alt="Logo">
            <CardComp
                class="mt-2 mx-auto single-post"
                picture="https://plus.unsplash.com/premium_photo-1683140655656-20448abc55da?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                parrafo="Publicación 1"
                :header="{ name: 'Natalia Ospina',
                picture: 'https://randomuser.me/api/portraits/women/66.jpg',
            }"
            likes="true"
            />
            <CardComp
                class="mt-2 mx-auto single-post"
                picture="https://images.unsplash.com/photo-1587620962725-abab7fe55159?q=80&w=1631&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                parrafo="Publicación 2"
                :header="{ name: 'Edilma Soto',
                picture: 'https://randomuser.me/api/portraits/women/43.jpg',
            }"
            likes="true"
            />
            <CardComp
                class="mt-2 mx-auto single-post"
                picture="https://images.unsplash.com/photo-1619410283995-43d9134e7656?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                parrafo="Publicación 3"
                :header="{ name: 'Javier Ospina',
                picture: 'https://randomuser.me/api/portraits/men/32.jpg',
            }"
            likes="true"
            />
            <CardComp
                class="mt-2 mx-auto single-post"
                picture="https://images.pexels.com/photos/3987066/pexels-photo-3987066.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
                parrafo="Publicación 4"
                :header="{ name: 'Fernando Patiño',
                picture: 'https://randomuser.me/api/portraits/men/67.jpg',
            }"
            likes="true"
            />
    </div>
</template>

<script>
    import CardComp from '../components/CardComp.vue'
    export default {
        name: 'PostsView',
        components: {
            CardComp
        }
    }
</script>

<style scoped>
    .posts {
        min-height: 60vh;
        max-width: 895px;
        margin: auto;
    }

    img {
        max-width: 200px;
        padding: 0.2rem;
    }
    .single-post {
        max-width: 550px;
    }
</style>