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
    <section id="footer">
        <!-- NEWS LETTER -->
        <div class="container">
            <div class="solition-wrap">
                <div class="row align-items-center justify-content-center">
                    <div class="col-lg-6">
                        <div class="content">
                            <h2 class="title">
                                Our news Letter
                            </h2>
                        </div>
                    </div>
                    <div class="col-lg-6">
                        <form>
                            <div class="input-ext">
                                <input type="text" placeholder="Enter Your Email">
                                <div class="icon-message">
                                    <svg class="svg-inline--fa fa-message" aria-hidden="true" focusable="false"
                                        data-prefix="fas" data-icon="message" role="img" xmlns="http://www.w3.org/2000/svg"
                                        viewBox="0 0 512 512" data-fa-i2svg="">
                                        <path fill="currentColor"
                                            d="M511.1 63.1v287.1c0 35.25-28.75 63.1-64 63.1h-144l-124.9 93.68c-7.875 5.75-19.12 .0497-19.12-9.7v-83.98h-96c-35.25 0-64-28.75-64-63.1V63.1c0-35.25 28.75-63.1 64-63.1h384C483.2 0 511.1 28.75 511.1 63.1z">
                                        </path>
                                    </svg>
                                    <!-- <i class="fas fa-message"></i> Font Awesome fontawesome.com -->
                                </div>
                            </div>
                            <button type="submit">Subscribe</button>
                        </form>
                    </div>

                </div>
            </div>
        </div>
    </section>
    <section class="footer-section footer-section-two">
        <div class="container">
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
            </nav>
            <!-- SEPARATORE -->
            <div class="footer-middle">
                <div class="footer-bottom">
                    <p>
                        Copyright © RaxG | Designed by <a href="#">NextGenerationDev</a>
                    </p>
                    <ul>
                        <li>
                            <a href="#">
                                <!-- <i class="fab fa-facebook"></i> Font Awesome fontawesome.com -->
                                facebook

                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <!-- <i class="fab fa-twitter"></i> Font Awesome fontawesome.com -->
                                twitter
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <!-- <i class="fab fa-linkedin"></i> Font Awesome fontawesome.com -->
                                linkedin
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <!-- <i class="fab fa-instagram"></i> Font Awesome fontawesome.com -->
                                instagram
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;

#footer {
    background-color: #202046;
    height: 480px;
}

nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px;
}

#logo {
    width: 190px;
}

.menu {
    display: flex;
    align-items: center;
}

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

li {
    margin: 0 20px;
}

ul {
    margin-top: 0;
    margin-bottom: 0;
}

.icon {
    background-color: white;
    width: 45px;
    height: 45px;
    margin: 0 10px;
    border-radius: 50px;
}

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

.footer-bottom {
    position: relative;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 20px 5px;
    border-top: 1px solid #9C9C9C;
}

.footer-bottom p a {
    color: #00AC4D;
}

.footer-bottom ul {
    display: flex;
}

.footer-bottom ul li {
    margin-right: 10px;
    padding-right: 10px;
}

.footer-bottom ul li a {
    text-transform: uppercase;
    font-size: 14px;
    color: #E6E7E8;
    display: block;
    width: 45px;
    height: 45px;
    line-height: 45px;
    border-radius: 50%;
    background: #202046;
    text-align: center;
    transition: all 0.3s;
    font-weight: 500;
}

.footer-middle {
    position: relative;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 160px 5px 40px;
}

.solition-wrap {
    background: #202046;
    padding: 60px 40px 60px;
    position: relative;
    margin-bottom: -85px;
    border-radius: 10px;
    z-index: 1;
}

.solition-wrap .content .title {
    font-size: 36px;
    font-weight: 700;
    color: #FFFFFF;
}

.solition-wrap form {
    background: #1A1935;
    padding: 10px 15px;
    border-radius: 100px;
    display: flex;
}

.solition-wrap form .input-ext {
    width: 85%;
    position: relative;
}

.solition-wrap form .input-ext input {
    border: none;
    outline: none;
    background: none;
    padding: 10px 0 0 40px;
}

.solition-wrap form .input-ext .icon-message {
    position: absolute;
    left: 17px;
    top: 13px;
}

.solition-wrap form .input-ext .icon-message svg {
    color: #00AC4D;
    font-size: 16px;
    overflow: visible;
    box-sizing: content-box;
}

.fa-message::before {

    content: "\f27a";

}

.svg-inline--fa {
    height: 1em;
    overflow: visible;
    vertical-align: -.125em;
}

.solition-wrap form button {
    border: none;
    outline: none;
    background: #00AC4D;
    padding: 12px 20px;
    font-size: 16px;
    font-weight: 500;
    border-radius: 100px;
    cursor: pointer;
}

.footer-section.footer-section-two::before {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    content: "";
    background: rgba(26, 25, 53, 0.7);
}

.footer-section.footer-section-two {
    background: url(../assets/img/footer-bg.png) no-repeat center center;
    background-size: cover;
    position: relative;
}
</style>