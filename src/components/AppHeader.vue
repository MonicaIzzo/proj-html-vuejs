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
        <nav>
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
                    <!-- ICONE -->
                    <div class="debug">
                        ICONE
                    </div>
                </nav>
            </div>
        </nav>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/scss/_vars.scss' as *;

#header {
    background-color: $bludark;
    height: 400px;
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
    font-size: 24px;
    text-decoration: none;
}

a .active {
    color: $verde;
}

li {
    margin: 0 20px;
}
</style>