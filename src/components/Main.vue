<template>
    <div class="hero">
        <img class="background" src="@/assets/img/background.svg" />
        <div class="container">
            <div class="main">
                <nav class="text-right" id="changeLanguage">
                    <ul class="list-inline">
                        <li class="list-inline-item"><a href="#" v-on:click.prevent="changeLanguage('en')">English</a></li>
                        <li class="list-inline-item"><a href="#" v-on:click.prevent="changeLanguage('ja')">日本語</a></li>
                        <li class="list-inline-item d-none"><a href="#" v-on:click.prevent="changeLanguage('cn')">简体中文</a></li>
                        <li class="list-inline-item d-none"><a href="#" v-on:click.prevent="changeLanguage('tw')">繁体中文</a></li>
                        <li class="list-inline-item d-none"><a href="#" v-on:click.prevent="changeLanguage('kr')">한국어</a></li>
                    </ul>
                    ※ Some pages are not translated yet.
                </nav>
                <div id="home">
                <h5 class="title">{{ $t("hyunheeLee") }}</h5>
                <h3>{{ $t("Software Developer") }}</h3>
                <ul class="links">
                    <li>
                        <a
                        class="link"
                        href="https://github.com/Ariakekoichi/"
                        target="_blank"
                        title="Hyunhee Lee GitHub"
                        >Github</a
                        >
                    </li>
                    <li>
                        <a
                        class="link"
                        href="https://www.linkedin.com/in/hyunhee1121/"
                        target="_blank"
                        title="Hyunhee Lee LinkedIn"
                        >LinkedIn</a
                        >
                    </li>
                    <li>
                        <a
                        class="link"
                        href="https://calendly.com/jipai1121"
                        target="_blank"
                        title="Hyunhee Lee Schedule a call"
                        >Schedule a call</a
                        >
                    </li>
                </ul>
                <a
                    class="btn"
                    href="mailto:jipai1121@gmail.com"
                    subject="subject text"
                    target="_blank"
                    title="Hyunhee Lee e-mail"
                    >Message Me</a
                >
                </div>
                <div id="content">
                    <h2 class="sub-title">About</h2>
                    <div style="white-space:pre-wrap; word-wrap:break-word;">
                        {{ $t("About") }}
                    </div>
                    <h2 class="sub-title">Career</h2>
                    Japan Apr. 2017 to Present
                    <div id="japanCareer" class="flex flex-wrap flex-jc-center row">
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-primary">
                                    <div class="card-body">
                                        <i class="fa fa-arrow-circle-right fa-5x float-right"></i>
                                        <h3 class="card-title">Smaregi Inc.</h3>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content. This one is a little because it has more text!</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body text-primary">
                                        <h3 class="card-title">Wow! #3</h3>
                                        <p class="card-text">Suprise this one has content on the back!</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-dark">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h3 class="card-title">AdInte Co. ltd.</h3>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Software Developer at Product Division</h3>
                                        <h4 class="card-title">Nov. 2020 to May 2021</h4>
                                        <p class="card-text">Suprise this one has more more more more content on the back!</p>

                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-danger">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h3 class="card-title">Cyber Port Inc.</h3>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Back</h3>
                                        <p class="card-text">Suprise this one has more more more more content on the back!</p>

                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-success">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h3 class="card-title">Livelynx Inc.</h3>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Back</h3>
                                        <p class="card-text">Suprise this one has more more more more content on the back!</p>

                                    </div>
                                </div>
                            </div>
                        </div>
                         <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-warning">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h3 class="card-title">Cross Games Inc.</h3>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Back</h3>
                                        <p class="card-text">Suprise this one has more more more more content on the back!</p>

                                    </div>
                                </div>
                            </div>
                        </div>
                    </div><!-- #japanCareer -->
                    South Korea Jan. 2010 to Jan. 2013
                    <div id="koreaCareer" class="flex flex-wrap flex-jc-center row">
                        <div class="flipper col-sm-4">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-dark">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h3 class="card-title">HanShinKiJeon Co., Ltd.</h3>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">Suprise this one has more more more more content on the back!
                                    <div class="card-body">
                                        <h3 class="card-title">Back</h3>
                                        <p class="card-text">Suprise this one has more more more more content on the back!</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flipper col-sm-4">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-warning">
                                    <div class="card-body">
                                        <i class="fa fa-search-plus fa-5x float-right"></i>
                                        <h3 class="card-title">Powertronics Co.,Ltd.</h3>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-dark text-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Back #2</h3>
                                        <p class="card-text">Suprise this one has content on the back!</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div><!-- #koreaCareer -->
                    <h2 class="sub-title">Education</h2>
                        <p>{{ $t("Education1-1") }}</p>
                        <p>{{ $t("Education1-2") }}</p>
                        <p>{{ $t("Education2-1") }}</p>
                        <p>{{ $t("Education2-2") }}</p>
                    <h2 class="sub-title">Personal Activities</h2>
                </div><!-- #content -->
            </div><!-- .main -->
            <div class="footer">
                <div class="copyright">© 2022 Hyunhee Lee made by <a
                    class="link"
                    href="https://vuejs.org/"
                    target="_blank"
                    title="Vue.js"
                    >Vue.js</a
                    >
                </div>
            </div><!-- .footer -->
        </div>
    </div>
</template>

<script>
export default {
  name: "Main",
  components: {},
  methods: {
    changeLanguage(lang) {
      this.$i18n.locale = lang;
    }
  }
};
</script>

<style scoped>
.background {
    position: absolute;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.container {
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    position: relative;
    max-width: 1480px;
    height: 100vh;
    margin: 0px auto;
    padding: 0px 20px 0px 20px;
}
.main {
    /*max-width: 678px;*/
    width: 100%;
    margin: 0 auto;
    padding-top: 70px;
    display: flex;
    flex-direction: column;
}
.title {
    font-size: 72px;
    font-weight: 900;
    line-height: 91px;
}
.sub-title {
    font-size: 36px;
    font-weight: 400;
    line-height: 45px;
    padding-top: 10px;
    border-bottom: 5px solid #444;
    margin-bottom: 15px;
    width: fit-content;
}
.btn {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 120px;
    height: 40px;
    background-color: #2f2f2f;
    border-radius: 8px;
    color: #fff;
    font-size: 14px;
    margin: 48px auto 0px;
}
.btn:hover {
    opacity: 0.8;
    transition: 0.5s;
}
.footer {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-bottom: 30px;
    max-height: 200px;
    height: 100%;
}
.links {
    display: flex;
    margin: auto;
    max-width: 536px;
    width: 100%;
    justify-content: space-between;
    font-size: 14px;
    line-height: 18px;
    font-weight: 400;
}
.link:hover {
    transition: 0s;
    font-weight: 700;
}
.copyright {
    font-size: 15px;
    margin: auto;
    margin: 0 auto;
}
#home {
    text-align: center;
    align-items: center;
}
#changeLanguage {
    width: 100%;
}
.flipper {
    min-height: 300px;
}

/* flip card*/
.card-flip > div {
  backface-visibility: hidden;
  transition: transform 300ms;
  transition-timing-function: linear;
  width: 100%;
  height: 100%;
  margin: 0;
  display: flex;
}

.card-front {
  transform: rotateY(0deg);
}

.card-back {
  transform: rotateY(180deg);
  position: absolute;
  top: 0;
}

.card-flip:hover .card-front {
  transform: rotateY(-180deg);
}
  
.card-flip:hover .card-back {
  transform: rotateY(0deg);
}

@media (max-width: 707px) {
  .main {
    padding-top: 50px;
  }
}
@media (max-width: 555px) {
    .main {
        padding-top: 40px;
    }
    .title {
        line-height: 70px;
    }
    .title {
        font-size: 65px;
        line-height: 60px;
    }
    .sub-title {
        font-size: 26px;
    }
    .btn {
        margin: 40px auto 70px;
    }
}
@media (max-width: 480px) {
    .title {
        font-size: 45px;
        line-height: 40px;
    }
    .btn {
        margin-bottom: 40px;
    }
    .links {
        flex-direction: column;
        align-items: center;
        gap: 15px;
    }
    .copyright {
        font-size: 8px;
        margin-top: 25px;
    }
}
</style>