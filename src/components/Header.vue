<template>
    <header class="container-fluid p-3">
            <div class="row justify-content-between align-items-center">
                <nav class="col-4">
                    <ul class="d-flex justify-content-evenly m-0">
                        <li v-for="(element, index) in navLink" :key="index">
                            <a :href="element.url">
                                <span class="me-1">{{element.title}}</span>
                                <font-awesome-icon icon="fa-solid fa-angle-down"/>
                            </a>
                        </li>
                    </ul>
                </nav>
                <div id="logo" class="col-2 text-center">
                    <img src="../assets/images/dark-logo.png" alt="">
                </div>
                <div class="col-4">
                    <font-awesome-icon icon="fa-solid fa-cart-shopping"/>
                    <font-awesome-icon icon="fa-solid fa-circle-user"/>
                    <div id="search" class="d-inline position-relative">
                        <input type="text" placeholder="Search..">
                        <span class="position-absolute">
                            <font-awesome-icon icon="fa-solid fa-magnifying-glass"/>
                        </span>
                    </div>
                </div>
            </div>
    </header>
</template>

<script>
export default {
    name: 'IndexHeader',
    data: function() {
        return {
            navLink: [
                {
                    title: 'Home',
                    url: '#',
                },
                {
                    title: 'Pages',
                    url: '#',
                },
                {
                    title: 'Courses',
                    url: '#',
                },
                {
                    title: 'Features',
                    url: '#',
                },
                {
                    title: 'Blog',
                    url: '#',
                },
                {
                    title: 'Shop',
                    url: '#',
                },
            ],
        };
    },
};
</script>

<style lang="scss" scoped>
    nav ul {
        list-style: none;
        li a {
            text-decoration: none;
            color: #6c6c6b;
            font-size: 0.5rem;
            span {
                font-size: 0.8rem;
            }
        }
    }
    div#logo img {
        width: 50%;
    }
    div#search {
        input {
            border: transparent;
            background-color: #e2e2e0;
        }
        span.position-absolute {
            color: #1fad95;
            right: 5%;
            top: -10%;
            cursor: pointer;
        }
    }
</style>