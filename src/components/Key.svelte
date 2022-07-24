<script lang="ts">
    export let theKey: string

    let theKeyIsPressed = (event: KeyboardEvent) => {
        console.log(event.key);
        if(event.key == theKey) console.log(theKey ,' is press');   
    }

</script>

<div class='kb-button' on:keypress={theKeyIsPressed}>
    {theKey}
</div>

<style>
    .kb-button{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 2rem;
        font-size: 2rem;
        padding: 0.5rem;
        background: white;
        color: black;
        border-radius: 8px;
    }
</style>