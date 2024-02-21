<template>
  <div>
    <section class="my-container">
      <section class="d-flex flex-wrap mt-5 costum-section">
        <div class="order-2 order-md-1 mb-3 mb-md-0 media">
          <h1>Jr. Full Stack</h1>
          <h1>Web Developer 👋🏻</h1>
          <p>Hi, I'm Damiano. A passionate Jr Full Stack <br>
          Web Developer based in Milan, Italy.</p>
          <div class="social">
            <a href="https://github.com/DamianoLunardo" target="_blank" ><i class="fa-brands fa-github icons"></i></a>
            <a href="https://www.linkedin.com/in/damiano-lunardo/" target="_blank" ><i class="fa-brands fa-linkedin icons"></i></a>  
          </div>
        </div>
        <div class="box box2 order-1 order-md-2 justify-content-end img_div"></div>
      </section>

      <section class="d-flex mt-5 mb-5">
        <div class="prova">
          Tech Stack:
          <div>
            <span style="color: Tomato;"><i class="fa-brands fa-html5 icons first_icon"></i></span> 
            <span style="color: rgb(65, 65, 245);"><i class="fa-brands fa-css3-alt icons"></i></span>
            <span style="color: rgba(223, 223, 56, 0.834);"><i class="fa-brands fa-js icons"></i></span>
            <span style="color: palevioletred;"><i class="fa-brands fa-sass icons"></i></span>
            <span style="color: green;"><i class="fa-brands fa-vuejs icons"></i></span>
            <span style="color: rgb(103, 10, 103);"><i class="fa-brands fa-bootstrap icons"></i></span>
            <span style="color: violet;"><i class="fa-brands fa-php icons"></i></span>
            <span style="color: red;"><i class="fa-brands fa-laravel icons"></i></span>
          </div>
        </div>
      </section>
    </section>
  </div>
</template>

<style scoped lang="scss">

.prova {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
  .costum-section {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .box {
    width: 400px;
    height: 400px;
    margin: 100px 0px 0px 170px;
    border: 5px solid black;
    border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
    animation: morph 8s ease-in-out infinite;

    @keyframes morph {
      0% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
      }
      50% {
        border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%;
        background-image: linear-gradient(45deg, #fa88ff, #2bd2ff 50%, #2bff88 90%);
      }
      100% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
      }
    }
  }

  .box2 {
    background: url(../img/ciao.jpeg) no-repeat;
    background-size: cover;
    background-blend-mode: multiply;
    animation: morphTwo 8s ease-in-out infinite 1s;

    @keyframes morphTwo {
      0% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
      }
      50% {
        border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%;
      }
      100% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
      }
    }
  }

  p {
    color: gray;
    font-size: 13px;
    font-weight: 200;
  }

  img {
    width: 300px;
    height: 300px;
  }

  .icons {
    font-size: 50px;
    margin-right: 20px;
  }

  .first_icon {
    margin-left: 20px;
  }

  h1 {
    font-size: 65px;
  }

  p {
    font-size: 20px;
  }

  @media (max-width: 1200px) {
    .box {
      width: 300px;
      height: 300px;
    }
  }

  @media (max-width: 991px) {
    .costum-section {
      flex-direction: column;
      text-align: center;

      .box {
        margin: 20px auto;
      }
    }

    .img_div {
      margin: 0 auto;
    }
  }

  @media (max-width: 768px) {
    .box {
      width: 200px;
      height: 200px;
    }

    .icons {
      font-size: 30px;
      margin-right: 10px;
     }

    .first_icon {
      margin-left: 10px;
    }

    p {
      text-align: center;
    }

    h1 {
      text-align: center;
      font-size: 40px;
    }

    .media {
      margin-top: 15px;
    }

    .social {
      display: flex;
      justify-content: center;
    }
  }
</style>
