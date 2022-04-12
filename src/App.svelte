<script>
  import Key from "./components/Key.svelte";
  let keys = "QWERTYUIOPÅASDFGHJKLÖÄZXCVBNM";
</script>

<main>
  <div class="titlebar">
    <h1 class="title">Rapple!</h1>
  </div>
  <div class="boxholder" />
  <div class="keyboard">
    {#each keys as key}
      <Key letter={key} />
    {/each}
  </div>
</main>

<style>
  main {
    text-align: center;
    max-width: 420px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .titlebar {
    margin: 10px;
    width: 100%;
  }
  .title {
    color: #ffa061;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
    margin: 0 auto;
  }
  .keyboard {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    width: 100%;
  }
</style>
