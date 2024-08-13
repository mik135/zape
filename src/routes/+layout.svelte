<script>
    import "../app.css";
</script>
  
<slot />

<style>
    :global(:root) {
        --font-karla: "Karla", sans-serif;
        --font-montserrat: "Montserrat", sans-serif;
        --font-playwrite: "Playwrite DK Uloopet", cursive;

        font-optical-sizing: auto;
    }
</style>