<script setup>
    const submit = console.log('submitted')
</script>

<template>

    <the-header/>

    <section class="mx-auto">
        <div class="max-w-xl mx-auto">
            <h1 class="text-center text-2xl font-thin tracking-widest">contact</h1>
            <p class="mt-8 mb-20 font-thin text-center">Pour toutes demandes contactez moi</p>

            <form action="https://formspree.io/f/xwkjoyep" method="POST" class="appearance-none">
                <div class="my-6">
                    <input type="text" name="name" required placeholder="Nom" class="w-full focus:outline-none w-auto">
                    <hr>
                </div>

                <div class="my-6">
                    <input type="email" name="email" required placeholder="Email" class="w-full focus:outline-none">
                    <hr>
                </div>

                <div class="my-6">
                    <input type="text" name="subject" placeholder="Objet" class="w-full focus:outline-none">
                    <hr>
                </div>

                <div class="mb-8">
                    <textarea name="message" required rows="6" maxlenght="255" class="w-full focus:outline-none" placeholder="Rédigez votre messsage ici ..."></textarea>
                    <hr>
                </div>

                <div class="flex justify-center">
                    <button @submit="submit" type="submit" class="border py-3 px-9 bg-black font-thin text-white tracking-wider">Envoyer</button>
                </div>
            </form>

        </div>
    </section>

    <the-footer/>

</template>

