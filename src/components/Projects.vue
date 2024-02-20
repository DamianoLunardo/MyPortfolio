<template>
    <container class="my-container costum-section" id="projects">
      <h3 class="color-text">PROJECTS</h3>
      <div class="grid">
        <div class="project">
          <div class="image-container">
            <img class="card-img-top" src="../img/campominato.png" alt="js-campominato-dom">
            <div class="overlay prova">
              <a class="personal" href="https://github.com/DamianoLunardo/js-campominato-dom" target="_blank"><i class="fa-brands fa-github icons"></i></a>
              <a class="personal" href="https://damianolunardo.github.io/js-campominato-dom/" target="_blank">Demo</a>
            </div>
          </div>
        </div>
        <div class="project">
          <div class="image-container">
            <img class="card-img-top" src="../img/spotify.png" alt="spotify">
            <div class="overlay">
              <a class="personal" href="https://github.com/DamianoLunardo/html-css-spotifyweb" target="_blank"><i class="fa-brands fa-github icons "></i></a>
              <a class="personal" href="https://main--subtle-cactus-e80215.netlify.app/" target="_blank">Demo</a>
            </div>
          </div>
        </div>
        <div class="project">
          <div class="image-container">
            <img class="card-img-top" src="../img/boolflix.png" alt="boolflix">
            <div class="overlay">
              <a class="personal" href="https://github.com/DamianoLunardo/vite-boolflix" target="_blank"><i class="fa-brands fa-github icons "></i></a>
              <a class="personal" href="https://damianoboolflix.netlify.app" target="_blank">Demo</a>
            </div>
          </div>
        </div>
        <div class="project">
          <div class="image-container">
            <img class="card-img-top" src="../img/wp.png" alt="whatapp">
            <div class="overlay">
              <a class="personal" href="https://github.com/DamianoLunardo/vue-boolzapp" target="_blank"><i class="fa-brands fa-github icons "></i></a>
              <a class="personal" href="https://main--damiwhats.netlify.app/" target="_blank">Demo</a>
            </div>
          </div>
        </div>
        <div class="project">
          <div class="image-container">
            <img class="card-img-top" src="../img/avada.png" alt="avada">
            <div class="overlay">
              <a class="personal" href="https://github.com/DamianoLunardo/proj-html-vuejs" target="_blank"><i class="fa-brands fa-github icons "></i></a>
              <a class="personal" href="https://main--damainoavada.netlify.app/" target="_blank">Demo</a>
            </div>
          </div>
        </div>
        <div class="project">
          <div class="image-container">
            <img class="card-img-top" src="../img/vueslider.png" alt="vue-slider">
            <div class="overlay">
              <a class="personal" href="https://github.com/DamianoLunardo/vue-slider" target="_blank"><i class="fa-brands fa-github icons "></i></a>
              <a class="personal" href="https://main--damianovueslider.netlify.app/" target="_blank">Demo</a>
            </div>
          </div>
        </div>
        <!-- Aggiungi gli altri progetti qui -->
      </div>
    </container>
  </template>

<style scoped lang="scss">
.grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 20px;
}

.project {
    position: relative;
}

.personal {
    color: red;
    font-size: 25px;
    font-weight: 200;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    opacity: 0;
    transition: opacity 0.3s ease;
}

.overlay:hover .personal {
    opacity: 1;
}

.overlay a:nth-child(2) {
  top: 60%;
}

.card-img-top {
    object-fit: cover;
    height: 300px;
    object-fit: cover;
    
}

.image-container {
    position: relative;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgb(36, 36, 190); 
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: opacity 0.3s ease;
    cursor: pointer;
}

.image-container:hover .overlay {
    opacity: 1;
}

.costum-section {
    padding: 60px;
}



@media (max-width: 800px) {
    .personal {
        font-size: 20px;
        font-weight: 200;
    }
}
</style>

