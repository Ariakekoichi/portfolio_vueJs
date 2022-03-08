<template>
    <div class="hero">
        <img class="background" src="@/assets/img/background.png" />
        <div class="container">
            <div class="main">
                <nav class="text-right" id="changeLanguage">
                    <ul class="list-inline">
                        <li class="list-inline-item text-center">
                            <a href="#" v-on:click.prevent="changeLanguage('en')">
                                <img src="@/assets/img/flag/us.png" style="height:30px">
                                <p>English</p>
                            </a>
                        </li>
                        <li class="list-inline-item text-center">
                            <a href="#" v-on:click.prevent="changeLanguage('ja')">
                                <img src="@/assets/img/flag/jp.png" style="height:30px">
                                <p>日本語</p>
                            </a>
                        </li>
                        <li class="list-inline-item text-center"><!-- d-none -->
                            <a href="#" v-on:click.prevent="changeLanguage('cn')">
                                <img src="@/assets/img/flag/cn.png" style="height:30px">
                                <p>简体中文</p>
                            </a>
                        </li>
                        <li class="list-inline-item text-center"><!-- d-none -->
                            <a href="#" v-on:click.prevent="changeLanguage('tw')">
                                <img src="@/assets/img/flag/tw.png" style="height:30px">
                                <p>繁体中文</p>
                            </a>
                        </li>
                        <li class="list-inline-item text-center"><!-- d-none -->
                            <a href="#" v-on:click.prevent="changeLanguage('kr')">
                                <img src="@/assets/img/flag/kr.png" style="height:30px">
                                <p>한국어</p>
                            </a>
                        </li>
                    </ul>
                    <p class="my-3">※ Some pages are not translated yet.</p>
                </nav>
                <div id="home">
                <h5 class="title">{{ $t("hyunheeLee") }}</h5>
                <h3 class="mb-4">{{ $t("Software Developer") }}</h3>
                <img src="@/assets/img/MyPhoto.png">
                <ul class="links">
                    <li>
                        <a
                        class="btn"
                        href="https://github.com/Ariakekoichi/"
                        target="_blank"
                        title="Hyunhee Lee GitHub"
                        >Github</a
                        >
                    </li>
                    <li>
                        <a
                        class="btn"
                        href="https://www.linkedin.com/in/hyunhee1121/"
                        target="_blank"
                        title="Hyunhee Lee LinkedIn"
                        >LinkedIn</a
                        >
                    </li>
                    <li>
                        <a
                        class="btn"
                        href="https://calendly.com/jipai1121"
                        target="_blank"
                        title="Hyunhee Lee Schedule a call"
                        >Schedule a call</a
                        >
                    </li>
                </ul>
                </div>
                <div id="content">
                    <h2 class="sub-title">About</h2>
                    <div style="white-space:pre-wrap; word-wrap:break-word;">
                        {{ $t("About") }}
                    </div>
                    <h2 class="sub-title">Career</h2>
                    <h3 style="border-bottom: 2px solid #444; width: fit-content; line-height: 45px;">Japan</h3>
                    <div id="japanCareer" class="flex flex-wrap flex-jc-center row">
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-primary">
                                    <div class="card-body">
                                        <i class="fa fa-arrow-circle-right fa-5x float-right"></i>
                                        <h3 class="card-title">Smaregi Inc.</h3>
                                        <h5 class="card-title">Jun. 2021 to Present</h5>
                                        <p class="card-title">Osaka, JAPAN</p>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content. This one is a little because it has more text!</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Software Developer at Development department</h3>
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
                                        <h5 class="card-title">Nov. 2020 to May 2021</h5>
                                        <p class="card-title">Kyoto, JAPAN</p>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Software Developer at Product Division</h3>
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
                                        <h5 class="card-title">Aug. 2019 to Oct. 2020</h5>
                                        <p class="card-title">Osaka, JAPAN</p>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Web Developer at Development department</h3>
                                        <p class="card-text">Developed landing page designs, e-commerce sites, an invitation-only shopping mall website and created Search Engine Optimisation (SEO) strategies</p>

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
                                        <h5 class="card-title">Sep. 2017 to May 2019</h5>
                                        <p class="card-title">Fukuoka, JAPAN</p>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Software Developer at System Integration Division</h3>
                                        <p class="card-text">Developed a SDN controller system and three graph programs using modern JavaScript library(react, redux) technologies</p>

                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-secondary">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h3 class="card-title">Cross Games Inc.</h3>
                                        <h5 class="card-title">Sep. 2016 to Jul. 2017</h5>
                                        <p class="card-title">Fukuoka, JAPAN</p>
                                        <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Game programmer at Development department</h3>
                                        <p class="card-text">Developed a volleyball game for smartphones on consignment using Unity</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div><!-- #japanCareer -->
                    <h3 style="border-bottom: 2px solid #444; width: fit-content; line-height: 45px;">South Korea</h3>
                    <div id="koreaCareer" class="flex flex-wrap flex-jc-center row">
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-info">
                                    <div class="card-body">
                                        <i class="fa fa-search-plus fa-5x float-right"></i>
                                        <h3 class="card-title">Powertronics Co.,Ltd.</h3>
                                         <h5 class="card-title">Aug. 2011 to Jan. 2013</h5>
                                        <p class="card-title">Seoul, SOUTH KOREA</p>
                                        <p class="card-text">* Worked as a factory worker as part of military service (Mar. 2010 to Jan. 2013) #2</p>
                                    </div>
                                </div>
                                <div class="card-back bg-dark text-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Factory worker at Manufacturing Team</h3>
                                        <p class="card-text">Led a team of four and managed antenna production, packaging and quality check, increased productivity about 33% by voluntarily creating a quality check manual</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-dark">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h3 class="card-title">HanShinKiJeon Co., Ltd.</h3>
                                        <h5 class="card-title">Jan. 2010 to Aug. 2011</h5>
                                        <p class="card-title">Seoul, SOUTH KOREA</p>
                                        <p class="card-text">* Worked as a factory worker as part of military service (Mar. 2010 to Jan. 2013) #1</p>
                                    </div>
                                </div>
                                <div class="card-back bg-dark text-white">
                                    <div class="card-body">
                                        <h3 class="card-title">Factory worker at Manufacturing Team</h3>
                                        <p class="card-text">Washed hard disk and printer components and checked the quality</p>
                                        <p class="card-text">Managed the molds that produced the hard disk and printer components</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div><!-- #koreaCareer -->
                    <h2 class="sub-title">Education</h2>
                        <div id="education" class="flex flex-wrap flex-jc-center row">
                            <div class="flipper col-sm-4 my-3">
                                <div class="card card-flip h-100">
                                    <div class="card-front">
                                        <div class="card-body text-center">
                                            <img src="@/assets/img/KyushuUniversity.png" class="thumbnail h-50">
                                            <i class="fa fa-search fa-5x float-right"></i>
                                            <h5 class="card-title my-3">Apr. 2013 to Mar. 2017</h5>
                                            <p class="card-title">Fukuoka, JAPAN</p>
                                            <p class="card-text">{{ $t("Education1-2") }}</p>
                                        </div>
                                    </div>
                                    <div class="card-back bg-white">
                                        <div class="card-body">
                                            <h3 class="card-title">{{ $t("Education1-1") }}</h3>
                                            <p class="card-text">{{ $t("Education1-3") }}</p>

                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="flipper col-sm-4 my-3">
                                <div class="card card-flip h-100">
                                    <div class="card-front">
                                        <div class="card-body text-center">
                                            <img src="@/assets/img/CUHK.png" class="thumbnail h-50">
                                            <i class="fa fa-search fa-5x float-right"></i>
                                            <h5 class="card-title my-3">Aug. 2016</h5>
                                            <p class="card-title">HONG KONG</p>
                                            <p class="card-text">{{ $t("Education2-2") }}</p>
                                        </div>
                                    </div>
                                    <div class="card-back bg-white">
                                        <div class="card-body">
                                            <h3 class="card-title">{{ $t("Education2-1") }}</h3>
                                            <p class="card-text">{{ $t("Education2-3") }}</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div><!-- #education -->
                    <h2 class="sub-title">Personal Activities</h2>
                        <div id="personalActivities" class="flex flex-wrap flex-jc-center row">
                            <div class="flipper col-sm-4 my-3">
                                <div class="card card-flip h-100">
                                    <div class="card-front">
                                        <div class="card-body text-center">
                                            <img src="@/assets/img/geikoOke.png" class="thumbnail h-50">
                                            <i class="fa fa-search fa-5x float-right"></i>
                                            <h5 class="card-title my-3">Geiko Oke</h5>
                                            <h5 class="card-title my-3">Apr. 2013 to Mar. 2017</h5>
                                            <p class="card-title">Fukuoka, JAPAN</p>
                                        </div>
                                    </div>
                                    <div class="card-back bg-white">
                                        <div class="card-body">
                                            <h3 class="card-title">Geiko Oke</h3>
                                            <p class="card-text">{{ $t("Education1-3") }}</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="flipper col-sm-4 my-3">
                                <div class="card card-flip h-100">
                                    <div class="card-front">
                                        <div class="card-body text-center">
                                            <img src="@/assets/img/hongdeng.jpg" class="thumbnail h-50">
                                            <i class="fa fa-search fa-5x float-right"></i>
                                            <h5 class="card-title my-3">福岡中国語学友会</h5>
                                            <h5 class="card-title my-3">2015 to 2019</h5>
                                            <p class="card-title">Fukuoka, JAPAN</p>
                                        </div>
                                    </div>
                                    <div class="card-back bg-white">
                                        <div class="card-body">
                                            <h3 class="card-title">福岡中国語学友会</h3>
                                            <p class="card-text">{{ $t("Education2-3") }}</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="flipper col-sm-4 my-3">
                                <div class="card h-100">
                                    <div class="card-front">
                                        <div class="card-body text-center">
                                            <img src="@/assets/img/CUHK.png" class="thumbnail h-50 figure">
                                            <i class="fa fa-search fa-5x float-right"></i>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div><!-- #personalActivities -->
                    <h2 class="sub-title">Certifications</h2>
                    <strong>日本</strong><br>
                    <p>・基本情報技術者</p>
                    <p>・色彩検定 2級</p>
                    <p>・ファイナンシャルプランナー 3級（日本FP協会）</p>
                    <strong>韓国</strong><br>
                    <p>・電子機器技能士</p>
                    <strong>語学その他</strong>
                    <p>・新日本語能力試験（JLPT）1級</p>
                    <p>・新漢語水平考試（HSK）6級</p>
                    <p>・TOEIC 825点</p>
                    <p>・MOS Excel 2013 Specialist</p>
                </div><!-- #content -->
            </div><!-- .main -->
            <div class="footer">
                <a
                    class="btn"
                    href="mailto:jipai1121@gmail.com"
                    subject="subject text"
                    target="_blank"
                    title="Hyunhee Lee e-mail"
                    >Message Me</a
                >
                <div class="copyright mt-5 mb-5">© 2022 Hyunhee Lee made by <a
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
    height: 300px;
}

.figure:hover {
    -webkit-transform: scale(1.1);
    transform: scale(1.1);
    -webkit-transition: -webkit-transform .5s;
    transition: -webkit-transform .5s;
    transition: transform .5s;
    transition: transform .5s,-webkit-transform .5s;
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