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
    display: flex;
    justify-content: center;
    color: white;
    background-color: #475569;
    padding: 13px;
    margin: 10%;
    border-radius: 10px;
  }
</style>
