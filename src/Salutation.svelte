<script>
  export let greeting = "";
  export let identify = "";
</script>

<style>
  h1 {
    font-size: 9rem;
    margin-bottom: 2.5rem;
  }

  h2 {
    font-size: 2.5rem;
    font-weight: normal;
  }

  @media screen and (max-width: 800px) {
    h1 {
      font-size: 15vw;
      margin-bottom: 1.5rem;
    }

    h2 {
      font-size: 2rem;
    }
  }
</style>

<h1>{greeting}</h1>
<h2>{identify}</h2>
