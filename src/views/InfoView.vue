<template>
    <div class="container pt-5">
        <div class="row">
            <div class="col-md-3 col-sm-6">
                <div class="cocktail-container">
                    <img src="../assets/cocktail1.jpg" alt="">
                    <div class="background"></div>
                    <div class="d-flex info flex-column h-100">
                        <h5>Naam</h5>
                        <p class="mt-auto">&euro;7.00</p>
                        <p class="">21%</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="cocktail-container">
                    <img src="../assets/cocktail2.jpg" alt="">
                    <div class="background"></div>
                    <div class="d-flex info flex-column h-100">
                        <h5>Naam</h5>
                        <p class="mt-auto">&euro;7.00</p>
                        <p class="">21%</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="cocktail-container">
                    <img src="../assets/cocktail3.jpg" alt="">
                    <div class="background"></div>
                    <div class="d-flex info flex-column h-100">
                        <h5>Naam</h5>
                        <p class="mt-auto">&euro;7.00</p>
                        <p class="">21%</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="cocktail-container">
                    <img src="../assets/cocktail1.jpg" alt="">
                    <div class="background"></div>
                    <div class="d-flex info flex-column h-100">
                        <h5>Naam</h5>
                        <p class="mt-auto">&euro;7.00</p>
                        <p class="">21%</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="cocktail-container">
                    <img src="../assets/cocktail2.jpg" alt="">
                    <div class="background"></div>
                    <div class="d-flex info flex-column h-100">
                        <h5>Naam</h5>
                        <p class="mt-auto">&euro;7.00</p>
                        <p class="">21%</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="cocktail-container">
                    <img src="../assets/cocktail3.jpg" alt="">
                    <div class="background"></div>
                    <div class="d-flex info flex-column h-100">
                        <h5>Naam</h5>
                        <p class="mt-auto">&euro;7.00</p>
                        <p class="">21%</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="cocktail-container">
                    <img src="../assets/cocktail3.jpg" alt="">
                    <div class="background"></div>
                    <div class="d-flex info flex-column h-100">
                        <h5>Naam</h5>
                        <p class="mt-auto">&euro;7.00</p>
                        <p class="">21%</p>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6">
                <div class="cocktail-container">
                    <img src="../assets/cocktail1.jpg" alt="">
                    <div class="background"></div>
                    <div class="d-flex info flex-column h-100">
                        <h5>Naam</h5>
                        <p class="mt-auto">&euro;7.00</p>
                        <p class="">21%</p>
                    </div>
                </div>
            </div>

        </div>
    </div>
</template>

<style scoped>
.info * {
    position: relative;
    z-index: 3;
    margin: 0
}

.info {
    padding: .4rem
}

.cocktail-container {
    margin-bottom: 1rem;
    position: relative;
    aspect-ratio: 1
}
.background {
    background-color: black;
    position: absolute;
    top: 0;
    width: 100%;
    aspect-ratio: 1;
    opacity: .3;
    z-index: 2;
}
.cocktail-container img {
    position: absolute;
    object-fit: cover;
    aspect-ratio: 1;
    width: 100%;
    z-index: 1;
}
</style>
  