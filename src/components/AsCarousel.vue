<template >
    <button class="carousel-btn btn-next">Next</button>

    <div class="carousel red">
        <div class="inner-carousel">
            <div class="card" v-for="card in cards" :key="card">
                {{ card }}
            </div>
        </div>
    </div>
    <button class="carousel-btn btn-prev">Prev</button>
</template>
<script lang="ts" setup>
const cards = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

</script>
<style lang="scss" scoped>
.carousel {
    display: flex;
    justify-content: center;
    width: 20rem;
    overflow: hidden;

    .inner-carousel {
        display: flex;
        white-space: nowrap;

        .card {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 4rem;
            height: 4rem;
            color: white;
            background-color: #39b1bd;
            border-radius: 1.2rem;
            margin-right: 0.5rem;
        }
    }
}

.carousel-btn {
    margin: 0 1rem;
}
</style>