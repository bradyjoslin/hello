<script>
  let salutation = "Hello!";
  let greeting = "I am Brady.";
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

  @media screen and (max-width: 992px) {
    h1 {
      font-size: 15vw;
      margin-bottom: 1.5rem;
    }

    h2 {
      font-size: 2rem;
    }
  }
</style>

<h1>{salutation}</h1>
<h2>{greeting}</h2>
