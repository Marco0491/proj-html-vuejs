<template>
    <section class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-12 text-center mb-4">
                <p class="text-uppercase my_gray">join maxcoach at best</p>
                <h1 class="text-capitalize">latest online <span class="my_green fw-lighter">courses</span></h1>
            </div>
            <div class="col-8">
                <div v-for="element in coursesList" :key="element.id" class="card d-inline-block m-2">
                    <div v-if="element.price == 0" id="tag" class="text-white fw-bold position-absolute top-0 end-0 p-1">
                        <span class="text-uppercase">free</span>
                    </div>
                    <img :src="require(`../../assets/images/${element.image}`)" class="card-img-top" :alt="element.title">
                    <div class="card-body">
                        <span class="my_green fw-bold fs-5">${{element.price}}.<span class="fs-6">00</span></span>
                        <h6 class="card-title mt-2 mb-4">{{element.title}}</h6>
                        <div class="card-text">
                            <span class="me-3">
                                <font-awesome-icon icon="fa-solid fa-file-lines" class="me-2"/>{{element.lessonsNumber}} Lessons
                            </span>
                            <span>
                                <font-awesome-icon icon="fa-solid fa-circle-user" class="me-2"/>{{element.studentsNumber}} Students
                            </span>
                        </div>
                    </div>
                </div>
                <div id="pointer" class="col-12 text-center mb-3">
                    <span v-for="(element, index) in coursesList" :key="index" class="d-inline-block rounded-circle me-3"></span>
                </div>
                <div class="row justify-content-center">
                    <div class="col-5 text-center">
                        <p class="my_gray">
                            Control your personal preference settings to get notified about appropriate courses. 
                            <a href="#">
                                View all courses 
                                <font-awesome-icon icon="fa-solid fa-arrow-right-long"/>
                            </a>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
name: 'CoursesSection',
    data: function() {
        return {
            coursesList: [
                {
                    id: 1,
                    title: 'Learning to Write as a Professional Author',
                    price: 40,
                    image: 'course-02-480x298.jpg',
                    lessonsNumber: 20,
                    studentsNumber: 50,
                },
                {
                    id: 2,
                    title: 'Customer-centric Info-tech Strategies',
                    price: 0,
                    image: 'stock-full-hd-03-480x298.jpg',
                    lessonsNumber: 24,
                    studentsNumber: 769,
                },
                {
                    id: 3,
                    title: 'Open Programming Courses for Everyone: Python',
                    price: 19,
                    image: 'stock-full-hd-04-480x298.jpg',
                    lessonsNumber: 17,
                    studentsNumber: 62,
                },
            ],
        };
    },
};
</script>

<style lang="scss" scoped>
@import '../../assets/styles/variables.scss';

    p {
        font-size: 0.7rem;
        line-height: 1.5rem;
    }

    div.card {
        width: 18rem;
        div#tag {
            font-size: 0.8rem;
            background-color: #ee7455;
        }
        div.card-text {
            font-size: 0.7rem;
            color: $brand_gray;
        }
    }
    div#pointer span {
        width: 7px;
        height: 7px;
        background-color: $brand_gray;
        cursor: pointer;
        filter: opacity(0.3);
        &:hover {
            width: 10px;
            height: 10px;
            background-color: black;
            filter: opacity(0.7);
        }
    }
    a {
        color: black;
    }
</style>
