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
                    <p class="my-3">※ {{ $t("NotTranslated") }}</p>
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
                    <h3 class="mb-3">Japan</h3>
                    {{ $t("About_Japan") }}
                    <div id="japanCareer" class="flex flex-wrap flex-jc-center row">
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-primary">
                                    <div class="card-body">
                                        <i class="fa fa-arrow-circle-right fa-5x float-right"></i>
                                        <h3 class="card-title">{{ $t("Smaregi Inc.") }}</h3>
                                        <h5 class="card-title">{{ $t("Jun. 2021 to Present") }}</h5>
                                        <p class="card-title">Osaka, JAPAN</p>
                                        <h5 class="card-text">{{ $t("Smaregi-1") }}</h5>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h4 class="card-text"><a href="https://smaregi.jp/">https://smaregi.jp/</a></h4>
                                        <p class="card-text mt-2">・{{ $t("Growth") }}</p>
                                        <p class="card-text">・{{ $t("Smaregi-2") }}</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-dark">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h3 class="card-title">{{ $t("AdInte Co. ltd.") }}</h3>
                                        <h5 class="card-title">{{ $t("Nov. 2020 to May 2021") }}</h5>
                                        <p class="card-title">Kyoto, JAPAN</p>
                                        <h5 class="card-text">Software Developer at Product Division</h5>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h4 class="card-title"><a href="https://adinte.co.jp/">https://adinte.co.jp/</a></h4>
                                        <h5 class="card-text mt-2">A. Yarn Trade System</h5>
                                        <p class="card-text">・Developed a yarn trade system that supports multiple languages: Japanese, Mandarin Chinese, and English using codeigniter PHP framework</p>
                                        <h5 class="card-text mt-2">B. Advertisement space management tool</h5>
                                        <p class="card-text">・Developed a tool that manages each store’s advertisement space information that used to be managed in Excel</p>
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
                                        <h5 class="card-text">Web Developer at Development department</h5>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h4 class="card-text"><a href="https://cb-port.com/">https://cb-port.com/</a></h4>
                                        <p class="card-text mt-2">Developed landing page designs, e-commerce sites, an invitation-only shopping mall website and created Search Engine Optimisation (SEO) strategies</p>
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
                                        <h5 class="card-text">Software Developer at System Integration Division</h5>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h4 class="card-text"><a href="https://livelynx.co.jp/">https://livelynx.co.jp/</a></h4>
                                        <p class="card-text mt-2">Developed a SDN controller system and three graph programs using modern JavaScript library(react, redux) technologies</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-secondary">
                                    <div class="card-body">
                                        <i class="fa fa-search fa-5x float-right"></i>
                                        <h4 class="card-title">Cross Games Inc.</h4>
                                        <h5 class="card-text">Sep. 2016 to Mar. 2017 Student Internship</h5>
                                        <h5 class="card-text">Apr. 2016 to Jul. 2017 Game Programmer</h5>
                                        <p class="card-title mt-2">Fukuoka, JAPAN</p>
                                        <h5 class="card-text">Game programmer at Development department</h5>
                                    </div>
                                </div>
                                <div class="card-back bg-white">
                                    <div class="card-body">
                                        <h4 class="card-text"><a href="https://www.cross-games.jp/">https://www.cross-games.jp/</a></h4>
                                        <p class="card-text mt-2">Developed a volleyball game for smartphones on consignment using Unity</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div><!-- #japanCareer -->
                    <h3 class="mb-3">South Korea</h3>
                    {{ $t("About_Korea") }}
                    <div id="koreaCareer" class="flex flex-wrap flex-jc-center row">
                        <div class="flipper col-sm-4 my-3">
                            <div class="card card-flip h-100">
                                <div class="card-front text-white bg-info">
                                    <div class="card-body">
                                        <i class="fa fa-search-plus fa-5x float-right"></i>
                                        <h3 class="card-title">Powertronics Co.,Ltd.</h3>
                                        <h5 class="card-title">Aug. 2011 to Jan. 2013</h5>
                                        <p class="card-title">Seoul, SOUTH KOREA</p>
                                        <h5 class="card-text">Factory worker at Manufacturing Team</h5>
                                    </div>
                                </div>
                                <div class="card-back bg-dark text-white">
                                    <div class="card-body">
                                        <h4 class="card-title"><a href="http://www.powertro.com/">http://www.powertro.com/</a></h4>
                                        <p class="card-text mt-2">・Worked as a factory worker as part of military service (Mar. 2010 to Jan. 2013)</p>
                                        <p class="card-text">・Led a team of four and managed antenna production, packaging and quality check, increased productivity about 33% by voluntarily creating a quality check manual</p>
                                        <p class="card-text">・Awarded as the best staff of 2012</p>
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
                                        <h5 class="card-text">Factory worker at Manufacturing Team</h5>
                                    </div>
                                </div>
                                <div class="card-back bg-dark text-white">
                                    <div class="card-body">
                                        <h4 class="card-title"><a href="http://www.hskj.co.kr/xe/">http://www.hskj.co.kr/xe/</a></h4>
                                        <p class="card-text mt-2">・Worked as a factory worker as part of military service (Mar. 2010 to Jan. 2013)</p>
                                        <p class="card-text">・Inspected parts of hard disk and printer</p>
                                        <p class="card-text">・Managed the molds that produced the hard disk and printer components</p>
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
                                            <p class="card-text">{{ $t("QU1-2") }}</p>
                                        </div>
                                    </div>
                                    <div class="card-back bg-white">
                                        <div class="card-body">
                                            <h3 class="card-title">{{ $t("QU1-1") }}</h3>
                                            <p class="card-text">{{ $t("QU2-1") }}</p>

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
                                            <h3 class="card-title">{{ $t("CHUK1-1") }}</h3>
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
                                            <h5 class="card-title my-3">{{ $t("GeikoOke") }}</h5>
                                            <h5 class="card-title my-3">{{ $t("GeikoOkePeriod") }}</h5>
                                            <p class="card-title">Fukuoka, JAPAN</p>
                                        </div>
                                    </div>
                                    <div class="card-back bg-white">
                                        <div class="card-body">
                                            <h3 class="card-title">{{ $t("GeikoOke") }}</h3>
                                            <p class="card-text">{{ $t("GeikoOkeDescription-1") }}</p>
                                            <p class="card-text">{{ $t("GeikoOkeDescription-2") }}</p>
                                            <p class="card-text">{{ $t("GeikoOkeDescription-3") }}</p>
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
                                            <h5 class="card-title my-3">{{ $t("福岡中国語学友会") }}</h5>
                                            <h5 class="card-title my-3">{{ $t("2015 to 2019") }}</h5>
                                            <p class="card-title">Fukuoka, JAPAN</p>
                                        </div>
                                    </div>
                                    <div class="card-back bg-white">
                                        <div class="card-body">
                                            <h3 class="card-title">{{ $t("福岡中国語学友会") }}</h3>
                                            <p class="card-text">{{ $t("福岡中国語学友会-1") }}</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="flipper col-sm-4 my-3">
                                <div class="card card-flip h-100">
                                    <div class="card-front">
                                        <div class="card-body text-center">
                                            <img src="@/assets/img/forestWitch.png" class="thumbnail">
                                            <i class="fa fa-search fa-5x float-right"></i>
                                        </div>
                                    </div>
                                    <div class="card-back bg-white">
                                        <div class="card-body">
                                            <h3 class="card-title">{{ $t("Forest Witch") }}</h3>
                                            <p class="card-text">{{ $t("Forest Witch Description-1") }}</p>
                                            <p class="card-text">{{ $t("Forest Witch Description-2") }}</p>
                                            <p class="card-text">{{ $t("Forest Witch Description-3") }}</p>
                                            <p class="card-text">{{ $t("Forest Witch Description-4") }}</p>
                                            <h3 class="card-title mt-2">{{ $t("Forest Witch Download") }}</h3>
                                            <p class="card-text"><a href="https://drive.google.com/file/d/18kXaHyKOn-Kr_TXmAltx72Xccr1h2YI5/view?usp=sharing">https://drive.google.com/file/d/18kXaHyKOn-Kr_TXmAltx72Xccr1h2YI5/view?usp=sharing</a></p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div><!-- #personalActivities -->
                    <h2 class="sub-title">{{ $t("Certifications") }}</h2>
                    <h5 class="my-2">Japan</h5>
                    <p>・{{ $t("基本情報技術者") }}</p>
                    <p>・{{ $t("色彩検定 2級") }}</p>
                    <p>・{{ $t("ファイナンシャルプランナー 3級") }}</p>
                    <h5 class="my-2">South Korea</h5>
                    <p>・{{ $t("전자기기기능사") }}</p>
                    <h5 class="my-2">Languages</h5>
                    <p>・{{ $t("JLPT Level 1") }}</p>
                    <p>・{{ $t("HSK Level 6") }}</p>
                    <p>・TOEIC 825</p>
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
    width: 150px;
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