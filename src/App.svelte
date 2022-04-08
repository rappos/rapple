<script>
  import Key from "./components/Key.svelte";
</script>

<main>
  <h1>Rapple!</h1>
  <div class="keyboard-row">
    <Key letter="Q" />
    <Key letter="W" />
    <Key letter="E" />
    <Key letter="R" />
    <Key letter="T" />
    <Key letter="Y" />
    <Key letter="U" />
    <Key letter="I" />
    <Key letter="O" />
    <Key letter="P" />
    <Key letter="Å" />
  </div>
  <div class="keyboard-row">
    <Key letter="A" />
    <Key letter="S" />
    <Key letter="D" />
    <Key letter="F" />
    <Key letter="G" />
    <Key letter="H" />
    <Key letter="J" />
    <Key letter="K" />
    <Key letter="L" />
    <Key letter="Ö" />
    <Key letter="Ä" />
  </div>
  <div class="keyboard-row">
    <Key letter="Z" />
    <Key letter="X" />
    <Key letter="C" />
    <Key letter="V" />
    <Key letter="B" />
    <Key letter="N" />
    <Key letter="M" />
  </div>
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 360px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }
  .keyboard-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
  }
</style>
