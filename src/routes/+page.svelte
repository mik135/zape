<script>
    import landingImg from "$lib/assets/bg-landing-2.jpg"
</script>


<main>
        <section class="p-5 flex flex-col items-center h-full w-full gap-5">
            <span class="mt-5 w-full">
                <h1 class="text-3xl text-white"><span class="text-pink-600 font-extrabold">Zap</span>e</h1>
                <p class="text-white">Dating for techies.</p>
            </span>

            <div class="bgHero">
                <!-- <div class="h-32 overflow-hidden">
                    <img src={landingImg} alt="">
                </div> -->
                <div class="w-full flex flex-col gap-5 mt-auto mb-16">
                    <h3 class="text-white text-5xl font-extrabold">Tired Of Swiping <span class="text-pink-500">Left?</span></h3>
                    <h5 class="text-xl text-white">You might be brilliant at building tech or creating art, but finding true love? That's a different algorithm. Let us help you find your perfect match.</h5>
                    <button class="btn border-0 w-56 bg-indigo-600 rounded-3xl text-xl text-white">Find My Match</button>
                </div>
            </div>
        </section>
    
</main>

<style lang="postcss">
    main {
        max-height: 100vh;
        overflow: hidden;
    }
    section {
        min-height: 100vh;
        /*  */
        background-size: contain;
    }

    .bgHero {
        background-image: url("$lib/assets/bg-landing-3.jpg");
        height: 90vh;
        padding: 15px;
        border-radius: 20px;
        background-size: contain;
        display: flex;
    }

    h1 {
        font-family: var(--font-playwrite);
    }

    button {
        font-family: var(--font-montserrat);
    }

    p {
        font-family: var(--font-karla);
    }

    h3 {
        font-family: var(--font-karla);
    }

    h5 {
        font-family: var(--font-montserrat)
    }
</style>
