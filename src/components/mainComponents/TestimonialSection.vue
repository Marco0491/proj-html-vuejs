<template>
    <section class="container-fluid">
        <div class="row justify-content-center mb-5">
            <div class="col-8">
                <div class="row mb-5">
                    <div class="col-6 p-5">
                        <span class="text-uppercase my_gray">testimonials</span>
                        <h1 class="text-capitalize m-3">why do people <span class="my_green fw-light">*hearts*</span> us?</h1>
                        <p class="my_gray">Seeking for verbals of our service quality? Fin them here. Everything is transparent and straightforward for your sense of justification.</p>
                        <a href="#" class="text-dark">View all <font-awesome-icon icon="fa-solid fa-arrow-right-long"/></a>
                    </div>
                    <div class="col-6">
                        <div id="testimonial-card" class="shadow-lg p-4">
                            <h6>Professional team of specialists and passionate mentors at reach</h6>
                            <p class="my_gray">I need to get a certification for English proficiency and Maxcoach is my best choice. Their tutors are smart and professional when dealing with students.</p>
                            <div class="d-flex">
                                <img class="rounded-circle me-4" src="../../assets/images/testimonial-avata-01.jpg" alt="testimonial avatar">
                                <div id="testimonial-info">
                                    <h6 class="text-uppercase">madley pondor</h6>
                                    <span class="my_gray">/ IT specialist</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="row bottom-row mb-5">
                    <div class="col-6 left-col position-relative">
                        <img class="position-absolute p-3" src="../../assets/images/home-3-team-image.png" alt="team image">
                        <img class="w-25 position-absolute" src="../../assets/images/maxcoach-shape-07.png" alt="maxcoach shape">
                        <img class="w-25 position-absolute" src="../../assets/images/maxcoach-shape-05.png" alt="maxcoach shape">
                        <img class="w-25 position-absolute" src="../../assets/images/maxcoach-shape-01.png" alt="maxcoach shape">
                        <img class="w-25 position-absolute" src="../../assets/images/svg-0.svg" alt="maxcoach shape">
                    </div>
                    <div class="col-6 right-col position-relative p-5">
                        <div class="my_circle position-absolute top-0 start-0 translate-middle"></div>
                        <span class="text-uppercase my_gray">everything in <span class="fw-bold">maxcoach</span></span>
                        <h1 class="text-capitalize m-3">we're here to <span class="my_green fw-light">transform</span> you!</h1>
                        <p class="my_gray">As learners, people can enjoy great companionship from MaxCoach mentors and educators. We can help you to develop and grow at your best.</p>
                        <button type="button" class="btn text-white px-4 py-2 fw-bold">Get Free Guide</button>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
name: 'TestimonialSection',
};
</script>

<style lang="scss" scoped>
@import '../../assets/styles/variables.scss';

    section {
        font-size: 0.8rem;
        div#testimonial-card {
            h6 {
                font-size: 0.9rem;
            }
            img {
                width: 13%;
            }
        }
        div.bottom-row div.left-col
        :nth-child(1) {
            width: 85%;
            z-index: 3;
        }
        div.bottom-row div.left-col
        :nth-child(2) {
            top: 85%;
            right: 37%;
        }
        div.bottom-row div.left-col
        :nth-child(3) {
            top: 25%;
            right: 95%;
            z-index: 2;
        }
        div.bottom-row div.left-col
        :nth-child(4) {
            top: 90%;
            right: 115%;
        }
        div.bottom-row div.left-col
        :nth-child(5) {
            top: 15%;
            right: 75%;
            filter: opacity(0.1);
            z-index: 1;
        }
        div.bottom-row div.right-col {
            div.my_circle {
            @include orange-circle;
            }
            button {
                font-size: 0.6rem;
                background-color: $brand_green;
            }
        }
    }
</style>
