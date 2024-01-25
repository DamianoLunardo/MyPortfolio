<template>
  <div class="container text-center padding_section">
    <div ref="lines" class="lines">
      <div class="line size_1">Hi,</div>
      <div ref="name" class="line name size_2">I'm Damiano</div>
      <div class="line size_3">Jr. Full Stack Web Developer,</div>
      <div class="line size_4">focused on recreating responsive web applications, mostly on the front-end side. I always love learning to use new updated and innovative tools! Here are some of my recent projects:</div>
      <button type="button" class="btn btn-secondary line mt-3 ">Projects</button>
    </div>
  </div>
</template>

<script>
import { gsap } from "gsap";

export default {
  mounted() {
    this.animateLines();
  },
  methods: {
    animateLines() {
      const lines = this.$refs.lines.querySelectorAll('.line');
      const name = this.$refs.name;

      
      gsap.set(lines, { x: -50, opacity: 0 });
      gsap.set(name, { color: "blue" });

      
      const timeline = gsap.timeline({ defaults: { ease: "power2.out" } });

      lines.forEach((line, index) => {
        if (index % 2 === 0) {
          timeline.fromTo(line, { x: -50, opacity: 0 }, { x: 0, opacity: 1, duration: 1, delay: index * 1 }, 0);
        } else {
          timeline.fromTo(line, { x: 50, opacity: 0 }, { x: 0, opacity: 1, duration: 1, delay: index * 2 }, 0);
        }
      });
    }
  }
};
</script>

<style scoped lang="scss">

.padding_section {
    padding-top: 200px;
    
}
.lines {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.line {
  margin-bottom: 10px;
}

.name {
  font-weight: bold;
}

.size_1{
    font-size: 30px;
}

.size_2 {
    font-size: 50px;
}

.size_3 {
    font-size: 40px;
}

.size_4 {
    font-size: 20px;
}
</style>