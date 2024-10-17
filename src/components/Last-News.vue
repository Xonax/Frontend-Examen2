<template>
    <div class="container">
        <div class="row">
            <div class="col-12 mb-5">
                <div class="news-item-container position-relative">
                    <img class="object-fit-cover w-100" src="../assets/Uitnodiging-feest-party.jpg" alt="Feest uitnodiging">
                    <div class="background"></div>
                    <h3>
                        Wij nodigen u uit!
                    </h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam aliquid sapiente maxime illum facilis. Laboriosam excepturi adipisci culpa, magnam aut qui corrupti, saepe repudiandae atque nisi molestias iure alias accusamus!</p>
                </div>
            </div>

            <div class="col-12 mb-5">
                <div class="news-item-container position-relative">
                    <img class="object-fit-cover w-100" src="../assets/istockphoto-1298329918-612x612.jpg" alt="Feest uitnodiging">
                    <div class="background"></div>
                    <h3>
                        Wij nodigen u uit!
                    </h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam aliquid sapiente maxime illum facilis. Laboriosam excepturi adipisci culpa, magnam aut qui corrupti, saepe repudiandae atque nisi molestias iure alias accusamus!</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

.news-item-container img {
    position: absolute;
    height: 100%;
    height: 100%;
    z-index: 1;
}

.news-item-container .background {
    background-color: black;
    height: 100%;
    width: 100%;
    opacity: .5;
    position: absolute;
    top: 0;
    z-index: 2;
}

.news-item-container h3 {
    position: relative;
    padding: 2rem;
    z-index: 3;
}

.news-item-container p {
    position: relative;
    padding: 2rem;
    padding-top: 5rem !important;
    margin: 0;
    z-index: 3;
}

</style>

<script>
export default {
    name: 'LastNews',
    components: {
        
    }
}

</script>