<template>
  <section class="principal">
    <navbar/>
    <section class="hero">
      <div class="left animate-left">
        <h1>Os stickers mais toppers da internet!</h1>
        <p class="animate-left">E mais baratos!</p>
        <div class="botoes animate-left-slow-2">
          <a href="#" v-scroll-to="'#generos'" class="btn-header">Conheça</a>
        </div>
      </div>
      <div class="right animate-right">
          <img src="../assets/images/rick-header.png" alt="">
      </div>
    </section>

    <section class="generos" id="generos">
      <ul class="grid">
        <li class="small animate-left" style="background-image: url(https://demo.tutorialzine.com/2016/06/freebie-landing-page-template-with-flexbox/assets/img/coast.jpg);"></li>
        <li class="large animate-right" style="background-image: url(https://demo.tutorialzine.com/2016/06/freebie-landing-page-template-with-flexbox/assets/img/island.jpg);"></li>
        <li class="large animate-left" style="background-image: url(https://demo.tutorialzine.com/2016/06/freebie-landing-page-template-with-flexbox/assets/img/balloon.jpg);"></li>
        <li class="small animate-right" style="background-image: url(https://demo.tutorialzine.com/2016/06/freebie-landing-page-template-with-flexbox/assets/img/mountain.jpg);"></li>
      </ul>
    </section>

    <footer>
      <ul>
          <li>
              <a href="#">
                  <i class="fa fa-twitter-square"></i>
              </a>
          </li>
          <li>
              <a href="#">
                  <i class="fa fa-facebook-square"></i>
              </a>
          </li>
      </ul>
    </footer>
  </section>
</template>

<script>
import navbar from '@/components/general/navbar'

export default {
  name: 'Home',
  components: {
    navbar
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hero {
  background: tomato;
  top: 50px;
  min-height: 100vh;

  display: flex;
}

.hero .left {
  margin-top: auto;
  margin-bottom: auto;
  margin-right: auto;
  margin-left: 25%;
  width: 500px;

  color: #fff;
}

.hero .left h1 {
  font-family: "GothamRnd-Medium", sans-serif;
  font-size: 45px;
  padding: 10px;
}

.hero .left p {
  font-family: "GothamRnd-Book", sans-serif;
  font-size: 20px;
  padding: 10px;
}

.hero .right {
  margin-top: auto;
  margin-bottom: auto;
  margin-right: 20%;
  margin-left: auto;

  /* width: 200px;
  height: 200px;
  background-color: teal; */
}
.hero .right img {
  width: 350px;
  height: auto;
}

.animate-left {
  position: relative;
  animation: animateleft 0.5s;
}
.animate-left-slow {
  position: relative;
  animation: animateleft 1.1s;
}
.animate-left-slow-2 {
  position: relative;
  animation: animateleft 1.2s;
}
@keyframes animateleft {
  from {
    left: -300px;
    opacity: 0;
  }
  to {
    left: 0;
    opacity: 1;
  }
}
.animate-right {
  position: relative;
  animation: animateright 0.7s;
}
@keyframes animateright {
  from {
    right: -300px;
    opacity: 0;
  }
  to {
    right: 0;
    opacity: 1;
  }
}
.botoes {
  margin-top: 30px;
  padding: 10px;
}
.botoes a {
  font-family: 'GothamRnd-Medium', sans-serif;
  text-transform: uppercase;
  font-size: 20px;
  border: none;
  width: 200px;
  outline:0 !important;
  cursor: pointer;
}
</style>
