<template>
    <div>
        <ul class="flex justify-center my-36">
          
            <nuxt-link to="andMore" 
            class="font-thin hover:font-normal tracking-wide">Mais aussi
            </nuxt-link>

            <nuxt-link to="about" 
            class="font-thin hover:underline underline-offset-4 mx-5 tracking-wide">
            A propos
            </nuxt-link>

            <nuxt-link to="contact" 
            class="font-thin hover:font-normal tracking-wide">Contact
            </nuxt-link>

            <a class="mx-5 ease-in duration-300" href="https://instagram.com/maevamue?igshid=YmMyMTA2M2Y=">
                <img class="w-6" src="../assets/icons/instagram.png" alt="">
            </a>
            <a href="https://etsy.com/fr/shop/MaevaMu">
                <img class="w-5" src="../assets/icons/etsy.png" alt="">
            </a>
        </ul>
    </div>

    <div class="flex justify-center">
        <img class="w-4" src="../assets/icons/droits-dauteur.png" alt="">
        <span class="text-xs">2023, Maëva Muësser</span>
    </div>
</template>