<template>
    <div class="hero">
        <img class="background" src="@/assets/img/background.svg" />
        <div class="container">
            <div class="main">
                <nav class="text-right">
                    <ul class="list-inline">
                        <li class="list-inline-item"><a href="#" v-on:click.prevent="changeLanguage('en')">English</a></li>
                        <li class="list-inline-item"><a href="#" v-on:click.prevent="changeLanguage('ja')">日本語</a></li>
                        <li class="list-inline-item"><a href="#" v-on:click.prevent="changeLanguage('cn')">简体中文</a></li>
                        <li class="list-inline-item"><a href="#" v-on:click.prevent="changeLanguage('tw')">繁体中文</a></li>
                        <li class="list-inline-item"><a href="#" v-on:click.prevent="changeLanguage('kr')">한국어</a></li>
                    </ul>
                    ※ Some pages are not translated yet.
                </nav>
                <h5 class="title">{{ $t("hyunheeLee") }}</h5>
                <h3>{{ $t("Software Developer") }}</h3>
                <ul class="links">
                    <li>
                        <a
                        class="link"
                        href="https://github.com/Ariakekoichi/"
                        target="__blank"
                        title="Hyunhee Lee GitHub(in preparation)"
                        >Github</a
                        >
                    </li>
                    <li>
                        <a
                        class="link"
                        href="https://www.linkedin.com/in/hyunhee1121/"
                        target="__blank"
                        title="Hyunhee Lee LinkedIn"
                        >LinkedIn</a
                        >
                    </li>
                    <li>
                        <a
                        class="link"
                        href="https://calendly.com/jipai1121"
                        target="__blank"
                        title="Hyunhee Lee Schedule a call"
                        >Schedule a call</a
                        >
                    </li>
                </ul>
                <a
                    class="btn"
                    href="mailto:jipai1121@gmail.com"
                    subject="subject text"
                    target="__blank"
                    title="Hyunhee Lee e-mail"
                    >Message Me</a
                >
                <h2 class="sub-title">About</h2>
                {{ $t("About") }}
                <h2 class="sub-title">Career</h2>
                <h2 class="sub-title">Education</h2>
                {{ $t("Education") }}
                <h2 class="sub-title">Personal Activities</h2>
            </div><!-- main -->
            <div class="footer">
                <div class="copyright">© 2022 Hyunhee Lee made by <a
                    class="link"
                    href="https://vuejs.org/"
                    target="__blank"
                    title="Vue.js"
                    >Vue.js</a
                    >
                </div>
            </div><!-- footer -->
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
  text-align: center;
  align-items: center;
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