<script>
    export let title
</script>

<p class="title">
    {@html title}
</p>

<style>
    .title{
        cursor: pointer;
        margin: 1rem 0;
        padding: 0.75rem 2rem;
        font-size: 3rem;
        line-height: 3.3rem;
        font-weight: 600;
        position: absolute;
        top: 10%;
        z-index: 99;
        color: white;
        background: #324b4a50;
        backdrop-filter: blur(5px);
        -webkit-backdrop-filter: blur(5px);
        border-radius: 1rem;
    }
</style>