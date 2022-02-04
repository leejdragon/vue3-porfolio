<template>
  <!-- HEADER -->
  <header class="l-header">
      <nav class="nav bd-grid">
          <div>
              <a href="#" class="nav__logo">JeongYong</a>
          </div>

          <div class="nav__menu" id="nav-menu" :class="{active: isActive}" @click="activate">
              <ul class="nav__list">
                  <li class="nav__item"><a href="#home" class="nav__link">Home</a></li>
                  <li class="nav__item"><a href="#about" class="nav__link">About</a></li>
                  <li class="nav__item"><a href="#skills" class="nav__link">Skills</a></li>
                  <li class="nav__item"><a href="#work" class="nav__link">Work</a></li>
                  <li class="nav__item"><a href="#contact" class="nav__link">Contact</a></li>
              </ul>
          </div>

          <div class="nav__toggle" id="nav-toggle">
              <i class='bx bx-menu'></i>
          </div>
      </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isActive : false
    }
  },
  methods:{
    activate() {
      this.isActive = false;
    }
  }
}
</script>

<style>
.l-header {
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  z-index: var(--z-fixed);
  background-color: #fff;
  box-shadow: 0 1px 4px rgba(146, 161, 176, 0.15);
}

.nav__logo {
  color: var(--second-color);
}

@media screen and (max-width: 767px) {
  .nav__menu {
    position: fixed;
    top: var(--header-height);
    right: -100%;
    width: 80%;
    height: 100%;
    padding: 2rem;
    background-color: var(--second-color);
    transition: .5s;
  }
}

.nav__list {
    display: flex;
    padding-top: 0;
  }

.nav__item {
  margin-bottom: var(--mb-4);
}

.nav__link {
  position: relative;
  color: #fff;
}

.nav__link:hover {
  position: relative;
}

.nav__link:hover::after {
  position: absolute;
  content: '';
  width: 100%;
  height: 0.18rem;
  left: 0;
  top: 2rem;
  background-color: var(--first-color);
}

/*Active menu*/
.active::after {
  position: absolute;
  content: '';
  width: 100%;
  height: 0.18rem;
  left: 0;
  top: 2rem;
  background-color: var(--first-color);
}

.nav__toggle {
  color: var(--second-color);
  font-size: 1.5rem;
  cursor: pointer;
}

/* NAV */
.nav {
  height: var(--header-height);
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-weight: var(--font-semi);
}

@media screen and (min-width: 768px) {
  .nav__item {
    margin-left: var(--mb-6);
    margin-bottom: 0;
  }
  .nav__link {
    color: var(--second-color);
  }
}
</style>