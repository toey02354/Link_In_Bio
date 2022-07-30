<script>
    export let link, linkName, logoSrc
</script>

<a class="link-container" href={link} target="_blank" rel="noopender noreferrer">
    <img src={logoSrc} alt="logo" class="logo" /> 
    <p>{linkName}</p>
</a>

<style>
    .link-container{
        cursor: pointer;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 8px;
        background: #95b1af70;
        width: 100%;
        margin: 0 1em;
        border-radius: 1.5rem;
        font-size: 1.25rem;
        font-weight: 600;
        letter-spacing: 0.12em;
        transition: all 0.12s ease-in ;
        backdrop-filter: blur(10px);
        box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.22);
    }

    .link-container:hover{
        background-color: #956E5E;
        color: #95B1AF;
    }
</style>