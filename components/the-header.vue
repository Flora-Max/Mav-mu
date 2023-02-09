<template>
    <nav class="w-auto flex justify-between items-center mx-10 mt-10">

        <div class="flex items-center">
            <img class="w-20" src="../assets/img/logo.png" alt="">
            <span class="items-center">Maëva Muësser</span>
        </div>

        

        <button class="w-4  md:hidden cursor-pointer">
            <img src="../assets/img/menu.png" alt="">
        </button>

        <ul class="hidden md:flex">
            <li class="mx-5">Instagram</li>
            <li class="mx-5">Facebook</li>
            <li class="mx-5">Etsy</li>
        </ul>
    </nav>

    <section id="mobile-menu" class="absolute w-full flex flex-col justify-content-center">
        <button class="self-end"></button>
    </section>
</template>