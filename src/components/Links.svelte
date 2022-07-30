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
        background: #95b1af70;
        width: 100%;
        justify-content: center;
        margin: 0 1em;
        border-radius: 1.5rem;
        /* transform: scaleX(90%); */
        font-size: 1.25rem;
        font-weight: 600;
        letter-spacing: 0.12em;
        transition: all 0.12s ease-in ;
        /* backdrop-filter: blur(15px); */
        box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.22);
        /* color: ; */
    }

    .link-container:hover{
        background-color: #956E5E;
        /* transform: scale(100%); */
        color: #95B1AF;
    }
</style>