<template>
  <div>
    <section class="navbar">
      <nav class="container">
        <div class="navbar-brand">
          <n-link class="navbar-item" to="/">
            <img
              class="logo"
              src="~static/mp-digital-logo-light.png"
              alt="Mark Perez Digital"
            />
          </n-link>

          <!-- Navbar Burger -->
          <span
            class="navbar-burger"
            @click="showNav = !showNav"
            data-target="navMenu"
          >
            <!-- hamburger lines -->
            <span></span>
            <span></span>
            <span></span>
          </span>
        </div>

        <!-- Navbar Menu -->
        <div id="navMenu" class="navbar-menu" :class="{ 'is-active': showNav }">
          <div @click="showNav = !showNav" class="navbar-end">
            <n-link class="navbar-item" to="/blog/">Blog</n-link>
            <n-link class="navbar-item" to="/CaseStudy/">Case Study</n-link>
            <n-link class="navbar-item" to="/gear/">Gear</n-link>
            <n-link class="navbar-item" to="/contact/">Contact</n-link>
            <a
              class="navbar-item"
              target="_blank"
              href="https://calendly.com/info-30250/discovery-call"
              ><button class="button is-rounded">Book a Call</button></a
            >
          </div>
        </div>
      </nav>
    </section>

    <hr />
  </div>
</template>

<script>
export default {
  data() {
    return {
      showNav: false
    }
  }
}
</script>

<style scoped>
hr {
  background-color: transparent;
}

a:hover,
a:active,
a:focus {
  color: #00c58e;
  background-color: transparent;
}

.button {
  letter-spacing: 1px;
  font-weight: bold;
  color: #fff;
  background-color: #2f495d;
  border-color: rgba(255, 255, 255, 0);
}

.logo {
  max-height: 3rem;
}

.navbar-menu {
  background-color:#00966b, #17ffbe;
}

.navbar {
  background-color: transparent;
  padding: 0 1rem;
  padding-top: 1rem;
  height: 4rem;
}

.navbar-item {
  font-size: 18px;
  padding-right: 2rem;
  color: #2f495d;
  font-weight: bolder;
  transition: 0.3s all;
}

.navbar-item:hover {
  color: #fff;
}

.navbar-brand {
  font-size: 22px;
}
</style>
