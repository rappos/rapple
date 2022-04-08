<script>
  export let letter = "A";
  export let letterColor = "rgb(203, 203, 203)";

  function ooops() {
    alert(letter);
  }
</script>

<main>
  <div on:click={ooops}>
    <p>{letter}</p>
  </div>
</main>

<style>
  div {
    background-color: rgb(203, 203, 203);
    padding: 0 10px 0 10px;
    margin: 0 auto;
  }
</style>
