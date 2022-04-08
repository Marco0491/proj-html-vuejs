<template>
    <section class="container-fluid">
        <div class="row justify-content-center mb-5">
            <div class="col-8">
                <div class="row">
                    <div class="left-col col-5 px-3">
                        <p class="my_gray text-uppercase">Everything in <span class="fw-bold">MaxCoach</span></p>
                        <h1 class="fs-1">Learn about our <span class="my_green fw-lighter">Work Coulture</span> at MaxCoach</h1>
                        <p class="my_gray">Spend some time to vist our website or head office and discover our current courses, enrollment procedure, and registration deadline. We're opening new classes every beginning of each month.</p>
                        <p class="my_gray">
                            Have a question? 
                            <a href="#" class="my_green">
                                Get free guide
                                <font-awesome-icon icon="fa-solid fa-arrow-right-long"/>
                            </a>
                        </p>
                    </div>
                    <div class="central-col col-1">
                        <div class="my_circle"></div>
                    </div>
                    <div class="right-col col-6 position-relative">
                        <img class="img-fluid position-relative rounded" src="../../assets/images/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="people who read">
                        <img class="position-absolute top-0 translate-middle rounded" src="../../assets/images/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="testimonial">
                        <img class="position-absolute" src="../../assets/images/maxcoach-shape-02.png" alt="maxcoach shape">
                        <img class="position-absolute top-0 translate-middle" src="../../assets/images/maxcoach-shape-07.png" alt="maxcoach shape">
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom-row row justify-content-center my_gray fw-bold">
            <div class="col-2 d-flex flex-column align-items-center">
                <span class="my_green fs-2">129+</span>
                <span class="text-uppercase">enrolled learners</span>
            </div>
            <div class="col-2 d-flex flex-column align-items-center">
                <span class="my_green fs-2">80</span>
                <span class="text-uppercase">finisced sessions</span>
            </div>
            <div class="col-2 d-flex flex-column align-items-center">
                <span class="my_green fs-2">4%</span>
                <span class="text-uppercase">satisfaction rate</span>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'LearnAboutSection',
}
</script>

<style lang="scss" scoped>
@import '../../assets/styles/variables.scss';

div.left-col {
    font-size: 0.8rem;
}

div.my_circle {
    @include orange-circle;
    transform: translate(-100%, -50%);
}

div.right-col img:nth-child(1) {
    z-index: 2;
}

div.right-col img:nth-child(2) {
    z-index: 3;
    width: 30%;
    left: 90%;
}

div.right-col img:nth-child(3) {
    z-index: 3;
    width: 20%;
    top: 80%;
    left: 65%;
}

div.right-col img:nth-child(4) {
    z-index: 1;
    width: 25%;
    left: 75%;
}

div.bottom-row {
    font-size: 0.7rem;
}

.my_green {
    color: $brand_green;
}

.my_gray {
    color: $brand_gray;
}
</style>
