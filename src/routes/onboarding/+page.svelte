<script>
    import Logo from '$lib/components/Logo.svelte'
    import RadioSelect from '$lib/components/RadioSelect.svelte'

    let position = $state(0)

    function navigateBack() {
        if(position > 0) {
            position--
        }
    }
</script>

<section class="p-5">
    <a href={position == 0 ? "/" : ""}><button onclick={navigateBack}>Go Back</button></a>
    <Logo />

    <form action="">
        {#if position == 0}
            
                <h2>Hi, let's do this! <br /> What's your gender?<h2>
            
            <div class="space-y-2">
                <RadioSelect content={"I'm a man"} name={"gender"} id={"man"}/>
                <RadioSelect content={"I'm a woman"} name={"gender"} id={"woman"}/>
            </div>
        {:else if position == 1}
            <h2>Step 2</h2>
            <button onclick={() => position++}>Next</button>
        {/if}
    </form> 
</section>

<style>
    section {
        background: radial-gradient(circle at left top, #eee , #7069ea);
        min-height: 100vh;
    }
</style>