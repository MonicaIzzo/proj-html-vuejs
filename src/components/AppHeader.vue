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
                        <div class="icon">search</div>
                        <div class="icon">icon</div>
                    </div>
                </nav>
            </div>
            <div class="banner">
                <span>WELCOME TO RAXG</span>
                <h1 class="title">
                    Are You ready For your next challenge?
                </h1>
                <div class="banner-btn-area">
                    <a href="#" class="btn">
                        Read More<!-- <i class="fa-solid fa-right-long"></i> Font Awesome fontawesome.com -->
                    </a>
                    <a href="#" class="video">
                        <!-- <i class="fas fa-play"></i> Font Awesome fontawesome.com -->
                        play
                    </a>
                </div>

            </div>

        </div>
        <div>
            <ul class="banner-social">
                <li>
                    <a href="#">
                        <!-- <i class="fab fa-facebook"></i> Font Awesome fontawesome.com --> F
                    </a>
                </li>
                <li class="bgshow">
                    <a href="#0">
                        <!-- <i class="fab fa-twitter"></i> Font Awesome fontawesome.com -->T
                    </a>
                </li>
                <li>
                    <a href="#">
                        <!-- <i class="fab fa-linkedin"></i> Font Awesome fontawesome.com -->L
                    </a>
                </li>
                <li>
                    <a href="#">
                        <!-- <i class="fab fa-instagram"></i> Font Awesome fontawesome.com -->
                        I
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

.bg-banner {
    height: 900px;
    background: url(../assets/img/banner1.png) no-repeat center center;
    background-size: cover;
    position: relative;

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

.btn {
    font-weight: 700;
    color: #1A1935;
    border-radius: 5px;
    line-height: 28px;
    padding: 12px 30px;
    background: #05CC7C;
    text-transform: capitalize;
    border: 1px solid #00AC4D;
    font-size: 16px;
    transition: all 0.3s;
}

.video {
    display: block;
    width: 60px;
    height: 60px;
    line-height: 60px;
    text-align: center;
    background: #05CC7C;
    border-radius: 50%;
}

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