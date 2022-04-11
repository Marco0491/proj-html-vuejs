<template>
    <section class="container-fluid py-5">
        <div class="row justify-content-center mb-5">
            <div class="col-12 text-center mb-4">
                <p class="text-uppercase my_gray">read for more joyment</p>
                <h1 class="text-capitalize">latest from <span class="my_green fw-lighter">our blogs</span></h1>
            </div>
            <div class="col-8">
                <div v-for="element in blogsList" :key="element.id" class="card d-inline-block m-2">
                    <img :src="require(`../../assets/images/${element.image}`)" class="card-img-top" :alt="element.title">
                    <div class="card-body">
                        <p class="my_gray text-uppercase fw-light m-0">artist</p>
                        <h6 class="card-title mt-2 mb-4">{{element.title}}</h6>
                        <div class="card-text">
                            <span class="me-3">
                                <font-awesome-icon icon="fa-solid fa-calendar" class="me-2"/>{{element.date}}
                            </span>
                            <span>
                                <font-awesome-icon icon="fa-solid fa-eye" class="me-2"/>{{element.views}} Views
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
name: 'BlogSection',
    data: function() {
        return {
            blogsList: [
                {
                    id: 1,
                    title: 'Brush Strokes Energize Trees in Paintings',
                    image: 'artist-blog-03-480x325.jpeg',
                    date: 'May 15, 2020',
                    views: 688,
                },
                {
                    id: 2,
                    title: 'Pocket-sized Notebooks Hold Miniature Paintings',
                    image: 'artist-blog-01-480x325.jpg',
                    date: 'May 16, 2020',
                    views: 603,
                },
                {
                    id: 3,
                    title: 'Connection Between Self-Portraits and Identity',
                    image: 'artist-blog-02-480x325.jpg',
                    date: 'May 15, 2021',
                    studentsNumber: 397,
                },
            ],
        };
    },
};
</script>

<style lang="scss" scoped>
@import '../../assets/styles/variables.scss';

section {
        background-color: #f8f8f8;
}

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
        &:hover {
            box-shadow: 10px 5px 5px rgba(0,0,0,0.2);
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
</style>
