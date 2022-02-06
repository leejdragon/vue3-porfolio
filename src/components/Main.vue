<template>
  <body>
    <main class="l-main">
        <!-- HOME -->
        <section class="home bd-grid" id="home">
            <div class="home__data">
                <h1 class="home__title">Hi,<br>I'am <span class="home__title-color">JeongYong</span><br> Frontend Developer</h1>

                <a href="#contact" class="button">Contact</a>
            </div>

            <div class="home__social">
                <a href="" class="home__social-icon"><i class='bx bxl-linkedin'></i></a>
                <a href="" class="home__social-icon"><i class='bx bxl-instagram' ></i></a> <box-icon type='logo' name='instagram'></box-icon>
                <a href="https://github.com/leejdragon" class="home__social-icon" target="_blank"><i class='bx bxl-github' ></i></a>
            </div>

            <div class="home__img">
              <img class="home__blob-img"  src="../assets/emoji.jpg"/> 
            </div>
        </section>

        <!-- ABOUT -->
        <section class="about section " id="about">
            <h2 class="section-title">About</h2>

            <div class="about__container bd-grid">
                <div class="about__img">
                    <img src="../assets/emoji.jpg" alt="">
                </div>
                
                <div>
                    <h2 class="about__subtitle">I'am JeongYong</h2>
                    <p class="about__text">high level experience in web frontend and <br> development knowledge, producing <br> quality work.</p>           
                </div>                                   
            </div>
        </section>

        <!-- SKILLS -->
        <section class="skills section" id="skills">
            <h2 class="section-title">Skills</h2>

            <div class="skills__container bd-grid">          
                <div>
                    <h2 class="skills__subtitle">Profesional Skills</h2>
                    <p class="skills__text">I learned JAVA at academy and studied Vue.js, a front-end framework by myself.</p>
                    <div class="skills__data">
                        <div class="skills__names">
                            <i class='bx bxl-html5 skills__icon'></i>
                            <span class="skills__name">HTML5</span>
                        </div>
                        <div class="skills__bar skills__html">

                        </div>
                        <div>
                            <span class="skills__percentage">95%</span>
                        </div>
                    </div>
                    <div class="skills__data">
                        <div class="skills__names">
                            <i class='bx bxl-css3 skills__icon'></i>
                            <span class="skills__name">CSS3</span>
                        </div>
                        <div class="skills__bar skills__css">
                            
                        </div>
                        <div>
                            <span class="skills__percentage">85%</span>
                        </div>
                    </div>
                    <div class="skills__data">
                        <div class="skills__names">
                            <i class='bx bxl-javascript skills__icon' ></i>
                            <span class="skills__name">JAVASCRIPT</span>
                        </div>
                        <div class="skills__bar skills__js">
                            
                        </div>
                        <div>
                            <span class="skills__percentage">65%</span>
                        </div>
                    </div>
                    <div class="skills__data">
                        <div class="skills__names">
                            <i class='bx bxl-vuejs skills__icon'></i>
                            <span class="skills__name">Vue.js</span>
                        </div>
                        <div class="skills__bar skills__ux">
                            
                        </div>
                        <div>
                            <span class="skills__percentage">85%</span>
                        </div>
                    </div>
                </div>
                
                <div>              
                    <img src="../assets/notebook.png" alt="" class="skills__img">
                </div>
            </div>
        </section>

        <!-- WORK -->
        <section class="work section" id="work">
            <h2 class="section-title">Work</h2>

            <div class="work__container bd-grid">
                <a href="" class="work__img">
                    <img src="../assets/work1.png" alt="">
                </a>
                <a href="" class="work__img">
                    <img src="../assets/work2.png" alt="">
                </a>
                <a href="" class="work__img">
                    <img src="../assets/work3.png" alt="">
                </a>
                <a href="" class="work__img">
                    <img src="../assets/work4.png" alt="">
                </a>
                <a href="" class="work__img">
                    <img src="../assets/work5.png" alt="">
                </a>
                <a href="" class="work__img">
                    <img src="../assets/work6.png" alt="">
                </a>
            </div>
        </section>

        <!-- CONTACT -->
        <section class="contact section" id="contact">
            <h2 class="section-title">Contact</h2>

            <div class="contact__container bd-grid">
                <form action="" class="contact__form">
                    <input type="text" placeholder="Name" class="contact__input">
                    <input type="mail" placeholder="Email" class="contact__input">
                    <textarea name="" id="" cols="0" rows="10" class="contact__input"></textarea>
                    <input type="button" value="Send" class="contact__button button">
                </form>
            </div>
        </section>
    </main>

  </body>
</template>

<script>
export default {
  name: 'Main',
  props: {
    msg: String
  },
}
</script>

<style>
/* CLASS CSS */
.section-title {
  position: relative;
  font-size: var(--h2-font-size);
  color: var(--first-color);
  margin-top: var(--mb-2);
  margin-bottom: var(--mb-4);
  text-align: center;
}

.section-title::after {
  position: absolute;
  content: '';
  width: 64px;
  height: 0.18rem;
  left: 0;
  right: 0;
  margin: auto;
  top: 2rem;
  background-color: var(--first-color);
}

.section {
  padding-top: 3rem;
  padding-bottom: 2rem;
}

/* LAYOUT */
.bd-grid {
  max-width: 1024px;
  display: grid;
  margin-left: var(--mb-2);
  margin-right: var(--mb-2);
}

/* Show menu */
.show {
  right: 0;
}

/* HOME */
.home {
  position: relative;
  row-gap: 5rem;
  padding: 4rem 0 5rem;
}

.home__data {
  align-self: center;
}

.home__title {
  font-size: var(--big-font-size);
  margin-bottom: var(--mb-5);
}

.home__title-color {
  color: var(--first-color);
}

.home__social {
  display: flex;
  flex-direction: column;
}

.home__social-icon {
  width: max-content;
  margin-bottom: var(--mb-2);
  font-size: 1.5rem;
  color: var(--second-color);
}

.home__social-icon:hover {
  color: var(--first-color);
}

.home__img {
  position: absolute;
  right: 0;
  bottom: 0;
  width: 260px;
}

.home__blob {
  fill: var(--first-color);
}

.home__blob-img {
  margin: 80px;
  width: 360px;
  border-radius: 70%;
}

/*BUTTONS*/
.button {
  display: inline-block;
  background-color: var(--first-color);
  color: #fff;
  padding: .75rem 2.5rem;
  font-weight: var(--font-semi);
  border-radius: .5rem;
  transition: .3s;
}

.button:hover {
  box-shadow: 0px 10px 36px rgba(0, 0, 0, 0.15);
}

/* ABOUT */
.about__container {
  row-gap: 2rem;
  text-align: center;
}

.about__subtitle {
  margin-bottom: var(--mb-2);
}

.about__img {
  justify-self: center;
}

.about__img img {
  width: 200px;
  border-radius: .5rem;
}

/* SKILLS */
.skills__container {
  row-gap: 2rem;
  text-align: center;
}

.skills__subtitle {
  margin-bottom: var(--mb-2);
}

.skills__text {
  margin-bottom: var(--mb-4);
}

.skills__data {
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
  font-weight: var(--font-semi);
  padding: .5rem 1rem;
  margin-bottom: var(--mb-4);
  border-radius: .5rem;
  box-shadow: 0px 4px 25px rgba(14, 36, 49, 0.15);
}

.skills__icon {
  font-size: 2rem;
  margin-right: var(--mb-2);
}

.bxl-html5 {
  color: orangered;
}

.bxl-css3 {
  color: blue;
}

.bxl-javascript {
  color: rgb(236, 221, 13);
}

.bxl-vuejs {
  color: #42b983;
}

.skills__names {
  display: flex;
  align-items: center;
}

.skills__bar {
  position: absolute;
  left: 0;
  bottom: 0;
  background-color: var(--first-color);
  height: .25rem;
  border-radius: .5rem;
  z-index: var(--z-back);
}

.skills__html {
  width: 95%;
}

.skills__css {
  width: 85%;
}

.skills__js {
  width: 65%;
}

.skills__ux {
  width: 85%;
}

.skills__img {
  border-radius: .5rem;
}

/* WORK */
.work__container {
  row-gap: 2rem;
}

.work__img {
  box-shadow: 0px 4px 25px rgba(14, 36, 49, 0.15);
  border-radius: .5rem;
  overflow: hidden;
}

.work__img img {
  transition: 1s;
}

.work__img img:hover {
  transform: scale(1.1);
}

/* CONTACT */
.contact__input {
  width: 100%;
  font-size: var(--normal-font-size);
  font-weight: var(--font-semi);
  padding: 1rem;
  border-radius: .5rem;
  border: 1.5px solid var(--second-color);
  outline: none;
  margin-bottom: var(--mb-4);
}

.contact__button {
  display: block;
  border: none;
  outline: none;
  font-size: var(--normal-font-size);
  cursor: pointer;
  margin-left: auto;
}

/* MEDIA QUERIES */
@media screen and (max-width: 320px) {
  .home {
    row-gap: 2rem;
  }
  .home__img {
    width: 200px;
  }
}

@media screen and (min-width: 576px) {
  .home {
    padding: 4rem 0 2rem;
  }
  .home__social {
    padding-top: 0;
    padding-bottom: 2.5rem;
    flex-direction: row;
    align-self: flex-end;
  }
  .home__social-icon {
    margin-bottom: 0;
    margin-right: var(--mb-4);
  }
  .home__img {
    width: 300px;
    bottom: 25%;
  }
  .about__container {
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    text-align: initial;
  }
  .skills__container {
    grid-template-columns: .7fr;
    justify-content: center;
    column-gap: 1rem;
  }
  .work__container {
    grid-template-columns: repeat(2, 1fr);
    column-gap: 2rem;
    padding-top: 2rem;
  }
  .contact__form {
    width: 360px;
    padding-top: 2rem;
  }
  .contact__container {
    justify-items: center;
  }
}

@media screen and (min-width: 768px) {
  body {
    margin: 0;
  }
  .section {
    padding-top: 4rem;
    padding-bottom: 3rem;
  }
  .section-title {
    margin-bottom: var(--mb-6);
  }
  .section-title::after {
    width: 80px;
    top: 3rem;
  }
  .nav {
    height: calc(var(--header-height) + 1.5rem);
  }
  
  .nav__toggle {
    display: none;
  }
  
  .home {
    padding: 8rem 0 2rem;
  }
  .home__img {
    width: 400px;
    bottom: 10%;
  }
  .about__container {
    padding-top: 2rem;
  }
  .about__img img {
    width: 300px;
  }
  .skills__container {
    grid-template-columns: repeat(2, 1fr);
    column-gap: 2rem;
    align-items: center;
    text-align: initial;
  }
  .work__container {
    grid-template-columns: repeat(3, 1fr);
    column-gap: 2rem;
  }
}

@media screen and (min-width: 992px) {
  .bd-grid {
    margin-left: auto;
    margin-right: auto;
  }
  .home {
    padding: 10rem 0 2rem;
  }
  .home__img {
    width: 450px;
  }
}
</style>
