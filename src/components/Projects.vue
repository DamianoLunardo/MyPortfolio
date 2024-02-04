<template>
    <container class="my-container costum-section">
        <h3 class="color-text">PROJECTS</h3>
        <div class="row justify-content-center">
            <div class="col-md-4">
                <div class="card" style="width: 18rem;">
                    <img class="card-img-top" src="../img/campominato.png" alt="js-campominato-dom">
                    <div class="card-body">
                        <a class="personal" href="https://github.com/DamianoLunardo/js-campominato-dom" target="_blank"><i class="fa-brands fa-github icons "></i></a>
                        <a class="personal" href="https://damianolunardo.github.io/js-campominato-dom/" target="_blank">Demo</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card" style="width: 18rem;">
                    <img class="card-img-top" src="../img/carosello.png" alt="js-array-objects-carousel">
                    <div class="card-body">
                        <a class="personal" href="https://github.com/DamianoLunardo/js-array-objects-carousel" target="_blank"><i class="fa-brands fa-github icons "></i></a>
                        <a class="personal" href="https://damianolunardo.github.io/js-array-objects-carousel/" target="_blank">Demo</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card" style="width: 18rem;">
                    <img class="card-img-top" src="../img/carosello.png" alt="js-array-objects-carousel">
                    <div class="card-body">
                        <a class="personal" href="https://github.com/DamianoLunardo/js-array-objects-carousel" target="_blank"><i class="fa-brands fa-github icons "></i></a>
                        <a class="personal" href="https://damianolunardo.github.io/js-array-objects-carousel/" target="_blank">Demo</a>
                    </div>
                </div>
            </div>
        </div>
    </container>
</template>

<style scoped lang="scss">
.personal {
    color: gray;
    font-size: 25px;
    font-weight: 200;

    &:hover {
        color: blue;
    }
}
.costum-section {
    padding: 60px;
}

.card-body {
    display: flex;
    justify-content: space-around;
    align-items: center;

    a {
        text-decoration: none;
        color: black;
    }
}

.card:hover{
    transform: scale(1.1);
    border-color: blue;
}

.card-img-top {
    width: 100%;
    height: 300px;
    object-fit: cover;
}

@media (max-width: 800px) {
    .card-body {
        flex-direction: column;

        a {
            margin-bottom: 10px;
        }
    }

    .row {
        justify-content: center;
    }

    .personal {
   
    font-size: 20px;
    font-weight: 200;
}

    
}

</style>
