<template>
    <section class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-8">
                <div class="row">
                    <div class="col-7 position-relative me-5">
                        <div class="video-preview p-2 position-relative">
                            <img class="img-fluid rounded" src="../../assets/images/stock-full-hd-11-670x450.jpg" alt="girl on the phone">
                            <img class="position-absolute top-50 start-50 translate-middle" src="../../assets/images/icon-youtube-play.png" alt="youtube icon">
                        </div>
                        <img class="first-shape position-absolute" src="../../assets/images/maxcoach-shape-07-150x150.png" alt="maxcoach shape">
                        <img class="second-shape position-absolute" src="../../assets/images/maxcoach-shape-05.png" alt="maxcoach shape">
                        <div class="svg w-25 position-absolute top-0">
                            <img class="img-fluid" src="../../assets/images/svg-0.svg" alt="maxcoach svg">
                        </div>
                    </div>
                    <div class="right-col col-4">
                        <div class="my_circle mb-2"></div>
                        <p class="text-uppercase fw-light">how we work</p>
                        <h1 class="text-capitalize">upgrade your skills <span class="fw-lighter my_green">upgrade your life</span></h1>
                        <p class="my_gray">Opening up more opportunities in front of you to get the ticket to more enjoyable door in life. Getting equipped with new skills for new sets of insights into your career. MaxCoach accompany learners in every stage of learning.</p>
                        <a href="#" class="fw-bold">
                                Download free guidebook
                                <font-awesome-icon icon="fa-solid fa-arrow-right-long"/>
                            </a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'UpgradeSkillSection',
}
</script>

<style lang='scss' scoped>
@import '../../assets/styles/variables.scss';

section {
    margin-bottom: 7rem;
}

div.video-preview {
    width: 100%;
    z-index: 3;
}

div.video-preview img:nth-child(2) {
    width: 15%;
    cursor: pointer;
}

img.first-shape {
    top: 75%;
    left: 75%;
    z-index: 2;
}

img.second-shape {
    top: 10%;
    transform: translateX(-45%);
    z-index: 2;
}

div.svg {
    filter: opacity(0.1);
    transform: translate(-30%, -50%);
    z-index: 1;
}

div.right-col {
    font-size: 0.7rem;
    div.my_circle {
        @include orange-circle;
    }
    a {
        color: black;
    }
}
</style>
