<template>
    <section class="container-fluid position-relative p-5">
        <div class="row flex-column align-items-center">
            <div class="my_circle position-absolute"></div>
            <div class="col-4 text-center p-4">
                <h1>Subscribe <span class="my_green fw-light">Newsletters</span></h1>
                <p class="my_gray fw-light">Enter your email address to register to our newsletter subscription delivered on a regular basis!</p>
            </div>
            <div class="col-4">
                <div class="input-group mb-3">
                    <input type="email" class="form-control bg-light my_gray fw-light" placeholder="Enter your email">
                    <span class="input-group-text text-white fw-bolder px-3 py-2" id="basic-addon2">Subscribe</span>
                </div>
            </div>
            <img class="first-shape position-absolute" src="../../assets/images/maxcoach-shape-09.png" alt="maxcoach shape">
            <img class="second-shape position-absolute" src="../../assets/images/maxcoach-shape-02.png" alt="maxcoach shape">
        </div>
    </section>
</template>

<script>
export default {
name: 'NewsletterSection',
}
</script>

<style lang="scss" scoped>
@import '../../assets/styles/variables.scss';

    div.my_circle {
        @include green-circle;
        top: 50%;
        left: 15%;
        filter: opacity(0.5);
    }

    p {
        font-size: 0.8rem;
        line-height: 1.5rem;
    }

    input {
        font-size: 0.7rem;
        border: transparent;
    }

    span#basic-addon2 {
        font-size: 0.7rem;
        background-color: $brand_green;
    }
    
    img.first-shape {
        width: 175px;
        right: 20%;
    }

    img.second-shape {
        width: 120px;
        top: 40%;
        right: 20%;
    }
</style>
