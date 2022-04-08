<template>
    <section id="jumbotron" class="position-relative">
        <img src="../assets/images/home-3-hero-bg.jpg" alt="jumbotron background">
        <div class="jumbotron-text text-center position-absolute">
            <span class="text-capitalize fs-4 fw-bold">commerce business</span>
            <h1 class="text-capitalize mb-4">distant mentoring program</h1>
            <button type="button" class="btn fw-bold">
                Download free guidebook
                <span id="arrow-right">
                    <font-awesome-icon icon="fa-solid fa-arrow-right-long"/>
                </span>
            </button>
        </div>
        <div id="jumbotron-inputs" class="d-flex flex-column rounded-start position-absolute">
            <span class="p-2">
                <font-awesome-icon icon="fa-solid fa-pen-to-square"/>
            </span>
            <span class="p-2">
                <font-awesome-icon icon="fa-solid fa-futbol"/>
            </span>
            <span class="p-2">
                <font-awesome-icon icon="fa-solid fa-book"/>
            </span>
            <span class="p-2">
                <font-awesome-icon icon="fa-solid fa-cart-shopping"/>
            </span>
        </div>
    </section>
</template>

<script>
export default {
    name: 'IndexJumbotron',
};
</script>

<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

section#jumbotron {
    height: 75vh;
    margin-bottom: 10rem;
    img {
        width: 100%;
        height: 100%;
    }
    div.jumbotron-text {
        color: white;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        h1 {
            font-size: 3rem;
            font-weight: 200;
        }
        button.btn {
            color: $brand_green;
            font-size: 0.7rem;
            background-color: white;
            padding: 0.5rem 2rem;
            &:hover {
                color: white;
                background-color: $brand_green;
            }
        }
    }
    div#jumbotron-inputs {
        color: $brand_gray;
        font-size: 0.8rem;
        background-color: white;
        top: 20%;
        right: 0;
    }
    div#jumbotron-inputs > * {
        cursor: pointer;
        &:hover {
            color: black;
        }
    }
}
</style>
