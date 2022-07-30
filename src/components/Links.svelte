<script>
    export let link, linkName
</script>

<a class="link-container" href={link} target="_blank" rel="noopender noreferrer">
    <!-- <img/> -->
    <p>{linkName}</p>
</a>

<style>
    .link-container{
        cursor: pointer;
        display: flex;
        gap: 4px;
        background: #95B1AF;
        width: 100%;
        justify-content: center;
        margin: 0 1em;
        border-radius: 1.5rem;
        /* transform: scaleX(90%); */
        font-size: 1.25rem;
        font-weight: 600;
        letter-spacing: 0.12em;
        transition: all 0.15s ease-in ;
        /* color: ; */
    }

    .link-container:hover{
        background-color: #956E5E;
        /* transform: scale(100%); */
        color: #95B1AF;
        outline: #95B1AF solid 4px;

    }
</style>