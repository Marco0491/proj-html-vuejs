<template>
    <header class="container-fluid p-3">
            <div class="row justify-content-between align-items-center">
                <nav class="col-4">
                    <ul class="d-flex justify-content-evenly m-0">
                        <li v-for="(element, index) in navLink" :key="index">
                            <a :href="element.url">
                                <span class="arrow me-1">{{element.title}}</span>
                                <font-awesome-icon icon="fa-solid fa-angle-down"/>
                            </a>
                        </li>
                    </ul>
                </nav>
                <div id="logo" class="col-2 text-center">
                    <img src="../assets/images/dark-logo.png" alt="">
                </div>
                <div class="col-4 text-center">
                    <span id="shopping-cart" class="position-relative">
                        <font-awesome-icon icon="fa-solid fa-cart-shopping"/>
                        <span id="cart-counter" class="position-absolute rounded-circle">{{shoppingCartCount}}</span>
                    </span>
                    <span id="user" class="mx-3">
                        <font-awesome-icon icon="fa-solid fa-circle-user"/>
                    </span>
                    <div id="search" class="d-inline position-relative">
                        <input type="text" class="rounded" placeholder="Search..">
                        <span class="lens position-absolute">
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
            shoppingCartCount: '0',
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
@import '@/assets/styles/variables.scss';

    nav ul {
        list-style: none;
        li a {
            text-decoration: none;
            color: $brand_gray;
            font-size: 0.5rem;
            span.arrow {
                font-size: 0.8rem;
            }
        }
    }

    div#logo img {
        width: 50%;
    }

    span#shopping-cart,span#user {
        cursor: pointer;
        color: $brand_gray;
    }

    span#cart-counter {
        width: 15px;
        height: 15px;
        color: white;
        text-align: center;
        line-height: 15px;
        font-size: 0.5rem;
        background-color: $brand_green;
        left: 70%;
        bottom: 70%;
    }

    div#search {
        input {
            width: 200px;
            border: transparent;
            background-color: #f5f5f5;
            font-size: 0.8rem;
            padding: 0.5rem 1rem;
        }
        span.lens {
            font-size: 0.8rem;
            color: $brand_green;
            right: 5%;
            top: 5%;
            cursor: pointer;
        }
    }
</style>
