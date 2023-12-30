<template>
    <div class="card">
      <CardHeader v-if="header" :header="header" />
      <div class="card-body">
              <h5 v-if="title" class="card-title">{{ title }}</h5>
                <p v-if="parrafo" class="card-text"> {{ parrafo }}</p>
                <img v-if="picture" :src="picture" alt="posts img" class="single-post">
                <ListGroup v-if="likes"/>
                <slot name="default"></slot>
                <div class="d-grid gap-2">
                  <botton v-for="btn in btns" :key="btn.txt" class="btn" :class="btn.class">{{ btn.txt }}</botton>
                  <slot name="footer"></slot>
                </div>
            </div>
        </div>
</template>

<script>
import CardHeader from './CardHeader.vue'
import ListGroup from './ListGroup.vue'
    export default {
      components: { CardHeader, ListGroup },
        name: "CardComp",
        props: ["title", "parrafo", "btns", "picture", "header", "likes",],
}
</script>

<style scoped>
    .card {
      border: none;
      box-shadow: 0 2px 4px rgb(0 0 0 / 10%), 0 8px 16px rgb(0 0 0 / 10%);
    }

    .card img {
      max-width: 100%;
    }
</style>
