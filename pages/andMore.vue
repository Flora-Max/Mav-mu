<template>

    <the-header/>

    <h1 class="text-center mb-12 font-thin text-3xl tracking-widest">Mais aussi</h1>

    <p class="text-center text-base font-thin tracking-widest mx-12 lg:mx-96 mb-12">Pour illuminer vos évênements, sublimer vos marchandises ou encore habiller votre intérieur je propose également des objets de décorations et des réalisations scénographiques.</p>

    <div class="container max-w-md lg:max-w-2xl mx-auto gap-x-44 grid grid-cols-1 sm:grid-cols-2">
        <img class="row-start-1 sm:mt-8" src="../assets/img3/les-fleurs.jpg" alt="illustration d'un bouquet de fleurs">
        <h2 class="row-start-2 font-thin italic text-xl tracking-widest mx-auto">Compositions florales</h2>
        <NuxtLink to="flowers" class="row-start-3 my-8 border mx-auto py-3 px-9 bg-black font-thin text-white tracking-wider">Découvrir</NuxtLink>

        <img class="row-start-4 sm:row-start-1 sm:col-start-2 mt-20 sm:mt-12" src="../assets/img3/vitrine.jpg" alt="illustration d'une vitrine">
        <h2 class="row-start-5 sm:row-start-2 sm:col-start-2 font-thin italic text-xl tracking-widest mx-auto">Vitrines</h2>
        <NuxtLink to="showcases" class="row-start-6 sm:row-start-3 sm:col-start-2 my-8 border mx-auto py-3 px-9 bg-black font-thin text-white tracking-wider">Découvrir</NuxtLink>
    </div>

    <the-footer/>
</template>