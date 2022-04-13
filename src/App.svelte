<script>
  import Key from "./components/Key.svelte";
  import Letterbox from "./components/Letterbox.svelte";
  let keys = "QWERTYUIOPÅASDFGHJKLÖÄZXCVBNM";
</script>

<main>
  <div class="titlebar">
    <h1 class="title">Rapple!</h1>
  </div>
  <div class="boxholder">
    {#each { length: 30 } as _, i}
      <Letterbox />
    {/each}
  </div>
  <div class="keyboard">
    {#each keys as key}
      <Key letter={key} />
    {/each}
  </div>
</main>

<style>
  main {
    text-align: center;
    width: 420px;
    max-height: 100%;
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
    color: white;
    text-transform: uppercase;
    font-size: 3em;
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
  .boxholder {
    display: grid;
    flex-grow: 1;
    gap: 10px;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(6, 1fr);
    width: 80%;
    margin-bottom: 30px;
  }
</style>
