<script>
    export let src
</script>

<!-- svelte-ignore a11y-img-redundant-alt -->
<img {src} alt="an image that passed in here">

<style>
    img{
        /* width: 100vw; */
        object-fit: cover;
        height: 50vh;
    }
</style>