<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand nav-link" href="#">
        <img src="../img/ciao.jpeg" width="70" height="70" class="d-inline-block align-top" alt="">
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link" href="">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Skill</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Projects</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
import { gsap } from "gsap";

export default {
  mounted() {
    
    const navLinks = this.$el.querySelectorAll('.navbar-nav .nav-link');

    
    gsap.set(navLinks, { opacity: 0, y: 20 });

    
    const timeline = gsap.timeline({ defaults: { ease: "power2.out" } });

    
    navLinks.forEach((link, index) => {
      timeline.to(link, { opacity: 1, y: 0, duration: 0.5, delay: index * 0.1 });
    });

    
    timeline.play();
  }
};
</script>

<style scoped lang="scss">

img {
  border-radius: 50%;
}

nav {
  font-size: 20px;
}
</style>