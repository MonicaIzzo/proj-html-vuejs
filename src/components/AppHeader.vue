<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'Home',
                    url: '#',
                    isActive: true
                },
                {
                    text: 'Pages',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'Tournament',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'Shop',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'Blog',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'Contact',
                    url: '#',
                    isActive: false
                },

            ]
        }
    }
}
</script>
<template>
    <section id="header">
        <div class="bg-banner">
            <div class="container">
                <!-- HEADER -->
                <nav>
                    <!-- LOGO -->
                    <div class="debug">
                        <div id="logo">
                            <a href="#" class="logo">
                                <img src="../assets/img/menulogo.png" alt="logo">
                            </a>
                        </div>
                    </div>
                    <!-- MENU -->
                    <div class="debug">
                        <div>
                            <ul class="menu">
                                <li v-for="link in links" :key="link.text"><a :href="link.url"
                                        :class="{ active: link.isActive }">{{
                                            link.text }}</a></li>
                            </ul>
                        </div>
                    </div>
                    <!-- ICONE -->
                    <div class="debug d-flex">
                        <div class="search-icon"><svg class="svg-inline--fa fa-magnifying-glass" aria-hidden="true"
                                focusable="false" data-prefix="fas" data-icon="magnifying-glass" role="img"
                                xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg="">
                                <path fill="#3C3C93"
                                    d="M500.3 443.7l-119.7-119.7c27.22-40.41 40.65-90.9 33.46-144.7C401.8 87.79 326.8 13.32 235.2 1.723C99.01-15.51-15.51 99.01 1.724 235.2c11.6 91.64 86.08 166.7 177.6 178.9c53.8 7.189 104.3-6.236 144.7-33.46l119.7 119.7c15.62 15.62 40.95 15.62 56.57 0C515.9 484.7 515.9 459.3 500.3 443.7zM79.1 208c0-70.58 57.42-128 128-128s128 57.42 128 128c0 70.58-57.42 128-128 128S79.1 278.6 79.1 208z">
                                </path>
                            </svg>
                        </div>
                        <div class="shop">
                            <svg class="svg-inline--fa fa-bag-shopping" aria-hidden="true" focusable="false"
                                data-prefix="fas" data-icon="bag-shopping" role="img" xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 448 512" data-fa-i2svg="">
                                <path fill="#3C3C93"
                                    d="M112 112C112 50.14 162.1 0 224 0C285.9 0 336 50.14 336 112V160H400C426.5 160 448 181.5 448 208V416C448 469 405 512 352 512H96C42.98 512 0 469 0 416V208C0 181.5 21.49 160 48 160H112V112zM160 160H288V112C288 76.65 259.3 48 224 48C188.7 48 160 76.65 160 112V160zM136 256C149.3 256 160 245.3 160 232C160 218.7 149.3 208 136 208C122.7 208 112 218.7 112 232C112 245.3 122.7 256 136 256zM312 208C298.7 208 288 218.7 288 232C288 245.3 298.7 256 312 256C325.3 256 336 245.3 336 232C336 218.7 325.3 208 312 208z">
                                </path>
                            </svg>
                            <span class="shop-rea">
                                0
                            </span>
                        </div>
                    </div>
                </nav>
            </div>
            <div class="banner text-center">
                <div class="row justify-content-center">
                    <div class="col-9">
                        <span>WELCOME TO RAXG</span>
                        <h1 class="title">
                            Are You ready For your next challenge?
                        </h1>
                    </div>
                </div>
            </div>
            <!-- PULSANTI -->
            <div class="container text-center mt-5">
                <div class="banner-btn-area row justify-content-center">

                    <div class="col-3">
                        <a href="#" class="btn">
                            Read More <svg class="svg-inline--fa fa-right-long" aria-hidden="true" data-prefix="fas"
                                data-icon="right-long" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M504.3 273.6l-112.1 104c-6.992 6.484-17.18 8.218-25.94 4.406c-8.758-3.812-14.42-12.45-14.42-21.1L351.9 288H32C14.33 288 .0002 273.7 .0002 255.1S14.33 224 32 224h319.9l0-72c0-9.547 5.66-18.19 14.42-22c8.754-3.809 18.95-2.075 25.94 4.41l112.1 104C514.6 247.9 514.6 264.1 504.3 273.6z">
                                </path>
                            </svg>
                        </a>
                    </div>
                    <div class="col-1">
                        <a href="#" class="video">
                            <svg class="svg-inline--fa fa-play" aria-hidden="true" focusable="false" data-prefix="fas"
                                data-icon="play" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"
                                data-fa-i2svg="">
                                <path fill="currentColor"
                                    d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z">
                                </path>
                            </svg><!-- <i class="fas fa-play"></i> Font Awesome fontawesome.com -->
                        </a>
                    </div>

                </div>
            </div>

        </div>
        <div>
            <!-- SOCIAL -->
            <ul class="banner-social">
                <li>
                    <a href="#">
                        <svg class="svg-inline--fa fa-facebook" aria-hidden="true" focusable="false" data-prefix="fab"
                            data-icon="facebook" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
                            data-fa-i2svg="">
                            <path fill="currentColor"
                                d="M504 256C504 119 393 8 256 8S8 119 8 256c0 123.8 90.69 226.4 209.3 245V327.7h-63V256h63v-54.64c0-62.15 37-96.48 93.67-96.48 27.14 0 55.52 4.84 55.52 4.84v61h-31.28c-30.8 0-40.41 19.12-40.41 38.73V256h68.78l-11 71.69h-57.78V501C413.3 482.4 504 379.8 504 256z">
                            </path>
                        </svg>
                    </a>
                </li>
                <li class="bgshow">
                    <a href="#">
                        <svg class="svg-inline--fa fa-twitter" aria-hidden="true" focusable="false" data-prefix="fab"
                            data-icon="twitter" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"
                            data-fa-i2svg="">
                            <path fill="currentColor"
                                d="M459.4 151.7c.325 4.548 .325 9.097 .325 13.65 0 138.7-105.6 298.6-298.6 298.6-59.45 0-114.7-17.22-161.1-47.11 8.447 .974 16.57 1.299 25.34 1.299 49.06 0 94.21-16.57 130.3-44.83-46.13-.975-84.79-31.19-98.11-72.77 6.498 .974 12.99 1.624 19.82 1.624 9.421 0 18.84-1.3 27.61-3.573-48.08-9.747-84.14-51.98-84.14-102.1v-1.299c13.97 7.797 30.21 12.67 47.43 13.32-28.26-18.84-46.78-51.01-46.78-87.39 0-19.49 5.197-37.36 14.29-52.95 51.65 63.67 129.3 105.3 216.4 109.8-1.624-7.797-2.599-15.92-2.599-24.04 0-57.83 46.78-104.9 104.9-104.9 30.21 0 57.5 12.67 76.67 33.14 23.72-4.548 46.46-13.32 66.6-25.34-7.798 24.37-24.37 44.83-46.13 57.83 21.12-2.273 41.58-8.122 60.43-16.24-14.29 20.79-32.16 39.31-52.63 54.25z">
                            </path>
                        </svg><!-- <i class="fab fa-twitter"></i> Font Awesome fontawesome.com -->
                    </a>
                </li>
                <li>
                    <a href="#">
                        <svg class="svg-inline--fa fa-linkedin" aria-hidden="true" focusable="false" data-prefix="fab"
                            data-icon="linkedin" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"
                            data-fa-i2svg="">
                            <path fill="currentColor"
                                d="M416 32H31.9C14.3 32 0 46.5 0 64.3v383.4C0 465.5 14.3 480 31.9 480H416c17.6 0 32-14.5 32-32.3V64.3c0-17.8-14.4-32.3-32-32.3zM135.4 416H69V202.2h66.5V416zm-33.2-243c-21.3 0-38.5-17.3-38.5-38.5S80.9 96 102.2 96c21.2 0 38.5 17.3 38.5 38.5 0 21.3-17.2 38.5-38.5 38.5zm282.1 243h-66.4V312c0-24.8-.5-56.7-34.5-56.7-34.6 0-39.9 27-39.9 54.9V416h-66.4V202.2h63.7v29.2h.9c8.9-16.8 30.6-34.5 62.9-34.5 67.2 0 79.7 44.3 79.7 101.9V416z">
                            </path>
                        </svg><!-- <i class="fab fa-linkedin"></i> Font Awesome fontawesome.com -->
                    </a>
                </li>
                <li>
                    <a href="#">
                        <svg class="svg-inline--fa fa-instagram" aria-hidden="true" focusable="false" data-prefix="fab"
                            data-icon="instagram" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"
                            data-fa-i2svg="">
                            <path fill="currentColor"
                                d="M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z">
                            </path>
                        </svg><!-- <i class="fab fa-instagram"></i> Font Awesome fontawesome.com -->
                    </a>
                </li>
            </ul>
        </div>



        <!-- LOGHI -->
        <div class="container text-center loghi-position">
            <div class="row loghi-row loghi">
                <div class="col">
                    <div class="logo-img">
                        <img src="../assets/img/1.png" alt="Logo For The King">
                    </div>
                </div>
                <div class="col">
                    <div class="logo-img">
                        <img src="../assets/img/2.png" alt="Logo For The King">
                    </div>
                </div>
                <div class="col">
                    <div class="logo-img">
                        <img src="../assets/img/3.png" alt="Logo Skullg">
                    </div>
                </div>
                <div class="col">
                    <div class="logo-img">
                        <img src="../assets/img/4.png" alt="Logo Panda">
                    </div>
                </div>
                <div class="col">
                    <div class="logo-img">
                        <img src="../assets/img/5.png" alt="Logo Witch">
                    </div>
                </div>
                <div class="col">
                    <div class="logo-img">
                        <img src="../assets/img/6.png" alt="Logo Astro">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;

#header {
    background-color: $bludark;
}

//-------------
//Immagine Hero
//-------------
.bg-banner {
    height: 900px;
    background: url(../assets/img/banner1.png) no-repeat center center;
    background-size: cover;
    position: relative;
}

.banner {
    margin-top: 150px;
}

.banner span {
    color: #00AC4D;
    text-transform: uppercase;
    font-weight: 600;
    display: block;
    font-size: 18px;
    margin-bottom: 15px;
}

.banner .title {
    font-size: 76px;
    color: #FFFFFF;
    text-transform: uppercase;
    font-weight: 700;
}


//-------------
//Menu di navigazione principale
//-------------
nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px;
}

.menu {
    display: flex;
    align-items: center;
}

//Logo
#logo {
    width: 190px;
}

// a del menu principale
a {
    color: white;
    font-weight: 700;
    text-transform: uppercase;
    font-size: 16px;
    text-decoration: none;
}

a .active {
    color: $verde;
}

// li del menu principale
ul {
    margin-top: 0;
    margin-bottom: 0;
}

li {
    margin: 0 20px;
}

// icone del menu
.shop {
    position: relative;
    width: 45px;
    height: 45px;
    line-height: 45px;
    border-radius: 50%;
    text-align: center;
    background: #FFFFFF;
    display: block;
}

.shop .shop-rea {
    position: absolute;
    top: -9px;
    right: -18px;
    background: #4350ff;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    line-height: 30px;
    text-align: center;
    color: #FFFFFF;
}

.search-icon {
    width: 45px;
    height: 45px;
    line-height: 45px;
    border-radius: 50%;
    text-align: center;
    background: #FFFFFF;
    display: block;
    position: relative;
    margin-right: 10px;
}

.fa-magnifying-glass::before {
    content: "\f002";
}





//-------------
// DIV centrale loghi
//-------------

// loghi del DIV centrale
.logo-img {
    width: 117px;
    height: 150px;
    text-align: center;
    margin: 0 auto;
}

.logo-img img {
    width: 100%;
    height: 100%;
    object-fit: contain;
}

.loghi-position {
    position: relative;
    top: -70px;
}

.loghi {
    background: #202046;
    padding: 40px 0;
    border-radius: 10px;
    width: 100%;
    z-index: 1;
    position: relative;
}

.loghi-row {
    max-width: 1140px;
    margin-right: auto;
    margin-left: auto;
    padding-right: 1rem;
    padding-left: 1rem;

}

//-------------
// SOCIAL
//-------------
.banner-social {
    position: absolute;
    top: 50%;
    left: 10%;
    transform: translate(-50%, -50%);
}

.banner-social li {
    margin-bottom: 12px;
    width: 45px;
    height: 45px;
    border-radius: 50%;
    line-height: 45px;
    background: #202046;
    text-align: center;
    transition: all 0.3s;
    cursor: pointer;
}
</style>