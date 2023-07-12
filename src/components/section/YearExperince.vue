<script>
</script>

<template>
    <section class="year-experince container-fluid">

        <div class="container">
            <div class="row g-5 justify-content-center align-items-center">
                <!-- colonna foto -->

                <div class="col">
                    <div class="about-thumb">
                        <div class="dots-about">
                            <img src="../../assets/img/exprience-shape.png" alt="about-dots">
                        </div>
                        <div class="bigsmall">
                            <img src="../../assets/img/shape1.png" alt="bigaboutimg">
                        </div>
                        <img src="../../assets/img/exprince.jpg" alt="a-img">
                        <div class="small-thumb">
                            <img src="../../assets/img/shape2.png" alt="small-img">
                        </div>
                    </div>
                </div>
                <!-- testo -->
                <div class="col">
                    <p><span class="subtitle">12 Year Experince</span></p>
                    <h1 class="title">We Are The Best Gaming Company</h1>
                    <p>Nulla quis lorem ut libero malesuada feugiat. Vivamus magna justo, lacinia eget consectetur sed,
                        convallis at
                        tellus. Cras ultricies ligula sed magna dictum porta.Praesent sapien massa, convallis a pellentesque
                        nec,
                        egestas non nisi praesent sapien massa ligula sed magna dictum porta. </p>
                    <p>Nulla quis lorem ut libero malesuada feugiat. Vivamus magna justo, lacinia eget consectetur sed,
                        convallis at
                        tellus. Cras ultricies ligulaa. </p>

                    <div class="about-list-area">
                        <ul>
                            <li>
                                <!-- <i class="fa-solid fa-check"></i> Font Awesome fontawesome.com -->Sed porttitor lectus
                                nibh.
                                Proin eget tortor
                                risus.
                            </li>
                            <li>
                                <!-- <i class="fa-solid fa-check"></i> Font Awesome fontawesome.com -->Praesent sapien
                                massa,
                                convallis a
                                pellentesque nec.
                                risus.
                            </li>
                            <li>
                                <!-- <i class="fa-solid fa-check"></i> Font Awesome fontawesome.com -->Praesent sapien
                                massa,
                                convallis a
                                pellentesque nec.
                                risus.
                            </li>
                            <li>
                                <!-- <i class="fa-solid fa-check"></i> Font Awesome fontawesome.com -->Praesent sapien
                                massa,
                                convallis a
                                pellentesque nec.
                                risus.
                            </li>
                        </ul>

                        <a href="#" class="btn">
                            Discover More
                            <!-- <i class="fa-solid fa-right-long"></i> Font Awesome fontawesome.com -->
                        </a>
                        <a href="#" class="video">
                            <!-- <i class="fas fa-play"></i> Font Awesome fontawesome.com -->
                        </a>

                    </div>
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/_vars.scss' as *;

.year-experince {
    background-color: $bludark;
}

p {
    margin-top: 0;
    margin-bottom: 1rem;
}

.about-list-area {
    margin-top: 30px;
    padding-bottom: 15px;
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
    width: 60px;
    height: 60px;
    line-height: 60px;
    text-align: center;
    background: #05CC7C;
    border-radius: 50%;
}

.about-thumb {
    max-width: 612px;
    margin: 0 60px 0 80px;
    position: relative;
}

.about-thumb .dots-about {
    position: absolute;
    top: -16px;
    left: -120px;
    width: 110px;
    height: 110px;
}

.about-thumb .dots-about img {
    width: 100%;
    height: 100%;
    object-fit: contain;
}

.about-thumb .bigsmall {
    max-width: 440px;
    position: absolute;
    top: -50px;
    left: -50px;
    z-index: -1;
}

.about-thumb .bigsmall img {
    width: 100%;
    height: 100%;
}

.about-thumb img {
    width: 100%;
    height: 100%;
    object-fit: contain;
}

.about-thumb .small-thumb {
    width: 260px;
    height: 260px;
    position: absolute;
    bottom: -31px;
    right: -31px;
    z-index: -1;
}

.about-thumb .small-thumb img {
    width: 100%;
    height: 100%;
}
</style>