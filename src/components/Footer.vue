<template>
    <footer class="container-fluid">
        <div class="row justify-content-center position-relative p-5">
            <div class="col-8">
                <div class="row">
                    <div class="col-6">
                        <h6 class="text-white text-capitalize">address</h6>
                        <p>382 NE 191st ST # 87394 Miami, FL 33179-3899</p>
                        <p>+1(305) 547-9909(9am - 5pm EST, Monday - Friday)</p>
                        <p>support@maxcoach.com</p>
                        <font-awesome-icon icon="fa-brands fa-facebook-square" class="fs-5 me-4"/>
                        <font-awesome-icon icon="fa-brands fa-twitter" class="fs-5 me-4"/>
                        <font-awesome-icon icon="fa-brands fa-instagram" class="fs-5 me-4"/>
                        <font-awesome-icon icon="fa-brands fa-linkedin" class="fs-5 me-4"/>
                    </div>
                    <div class="col-6">
                        <div class="row">
                            <div class="col-4">
                                <h6 class="text-white text-capitalize">explore</h6>
                                <ul class="p-0">
                                    <li v-for="element in exploreLink" :key="element.title">
                                        <a :href="element.url">{{element.title}}</a>
                                    </li>
                                </ul>
                            </div>
                            <div class="col-4">
                                <ul class="p-0 mt-4">
                                    <li v-for="element in contactLink" :key="element.title">
                                        <a :href="element.url">{{element.title}}</a>
                                    </li>
                                </ul>
                            </div>
                            <div class="col-4">
                                <h6 class="text-white text-capitalize">information</h6>
                                <ul class="p-0">
                                    <li v-for="element in infoLink" :key="element.title">
                                        <a :href="element.url">{{element.title}}</a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="col-12 text-center mt-5">
                        <p class="text-capitalize mb-0">2020 maxcoach. all rights reserved</p>
                    </div>
                </div>
            </div>
            <div id="back-on-top" class="position-absolute">
                <font-awesome-icon icon="fa-solid fa-arrow-up-long"/>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'IndexFooter',
    data: function() {
        return {
            exploreLink: [
                {
                    title: 'start here',
                    url: '#',
                },
                {
                    title: 'blog',
                    url: '#',
                },
                {
                    title: 'about us',
                    url: '#',
                }
            ],
            contactLink: [
                {
                    title: 'success story',
                    url: '#',
                },
                {
                    title: 'courses',
                    url: '#',
                },
                {
                    title: 'contact us',
                    url: '#',
                }
            ],
            infoLink: [
                {
                    title: 'membership',
                    url: '#',
                },
                {
                    title: 'purchase guide',
                    url: '#',
                },
                {
                    title: 'privacy policy',
                    url: '#',
                },
                {
                    title: 'terms of service',
                    url: '#',
                }
            ]
        }
    }
};
</script>

<style lang="scss" scoped>
@import '../assets/styles/variables.scss';

footer {
    background-color: #171621;
    color: $brand_gray;
    ul {
        list-style: none;
        li a {
            text-decoration: none;
            color: $brand_gray;
            font-size: 0.7rem;
        }
    }
    p {
        font-size: 0.7rem;
    }
    div#back-on-top {
        width: 40px;
        height: 40px;
        text-align: center;
        line-height: 40px;
        color: white;
        background-color: $brand_green;
        border-radius: 50%;
        right: 2rem;
        bottom: 2rem;
    }
}
</style>
