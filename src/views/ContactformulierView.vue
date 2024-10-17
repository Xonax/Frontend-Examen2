<template>
    <div class="container pt-5">
        <div class="row">
            <div class="col-md-5 offset-md-1">
                <h3 class="pb-3">Wil je contact met ons?</h3>
                <form action="" class="d-flex flex-column">
                    <input type="text" placeholder="Aanhef*" required>
                    <input type="text" placeholder="Naam*" required>
                    <input type="email" placeholder="E-mailadres*" required>
                    <input type="number" placeholder="Telefoonnummer*" required>
                    <input class="vraag" type="text" placeholder="Vraag/opmerking*" required>
                    <span class="d-flex">
                        <input class="checkbox me-1" type="checkbox">
                        <p>Aanmelden voor de nieuwsbrief</p>
                    </span>
                    <input type="submit">
                </form>
            </div>
            <div class="col-md-4 offset-md-1 d-flex align-items-center">
                <img class="w-100 object-fit-cover" src="../assets/Uitnodiging-feest-party.jpg" alt="Uitnodiging feest">
            </div>
        </div>
    </div>
</template>
  
<style scoped >
input {
    margin-bottom: 1rem;
}
.vraag {
    height: 14rem;
    border-radius: 14px !important;
}
input:not([type="checkbox"]) {
  border-radius: 50rem;
  border: none;
  width: 14rem;
  min-width: 2rem;
}
</style>