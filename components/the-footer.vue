<template>
    <div>
        <ul class="flex justify-center my-36">
            <nuxt-link to="about" 
            class="font-thin hover:underline underline-offset-4">
            A propos
            </nuxt-link>

            <nuxt-link to="vitrines" 
            class="font-thin hover:font-normal mx-5">Vitrines
            </nuxt-link>

            <a class="mx-5 ease-in duration-300" href="https://instagram.com/maevamue?igshid=YmMyMTA2M2Y=">
                <img class="w-7" src="../assets/icons/instagram.png" alt="">
            </a>
            <a class="mx-5" href="https://etsy.com/fr/shop/MaevaMu">
                <img class="w-7" src="../assets/icons/etsy.png" alt="">
            </a>
        </ul>
    </div>

    <div class="flex justify-center">
        <img class="w-4" src="../assets/icons/droits-dauteur.png" alt="">
        <span class="text-xs">2023, Maëva Muësser</span>
    </div>
</template>