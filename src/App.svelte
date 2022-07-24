<script lang="ts">
  import Key from './components/Key.svelte'

  let firstRow = ['Q','W','E','R','T','Y', 'U', 'I', 'O', 'P', '[', ']']

  let handleKeyPressDown = (event: KeyboardEvent) => {
    console.log('key down',event.key);
  }
  let handleKeyPressUp = (event: KeyboardEvent) => {
    console.log('key up',event.key);
  }

  addEventListener('keydown', handleKeyPressDown)
  addEventListener('keyup', handleKeyPressUp)

</script>

<div>
  <div class="wrapper">
    <div class="keeb-row">
      {#each firstRow as key}
        <Key theKey={key}></Key>
      {/each}
    </div>
  </div>
</div>

<style>
  .wrapper{
    display: flex;
    flex-direction: column;
    gap: 8px;
  }
  .keeb-row{
    display: flex;
    gap: 8px
  }
  
</style>