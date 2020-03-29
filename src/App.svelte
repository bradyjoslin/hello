<script>
  import Salutation from "./Salutation.svelte";
  import Portrait from "./Portrait.svelte";
  import Bio from "./Bio.svelte";
  import Links from "./Links.svelte";

  let greeting = "Hello!";
  let identify = "I am Brady.";
  let image_url = "./static/images/portrait.jpg";
</script>

<style>
  :global(body) {
    color: #eee;
    background-color: #424bb2;
    font-family: "Roboto", "Helvetica Neue", "Segoe UI", Helvetica, Arial,
      sans-serif;
  }

  main {
    display: flex;
    vertical-align: middle;
    margin-top: 10%;
  }

  main > div {
    flex: 50%;
  }

  main .left {
    text-align: center;
  }

  main .right {
    margin-right: 4rem;
  }

  main :global(a) {
    color: #eee;
  }

  main :global(a:hover) {
    color: #b2a842;
  }

  main a {
    text-decoration: underline;
  }

  @media screen and (max-width: 800px) {
    main {
      flex-direction: column;
      margin-top: 10%;
    }
    main .right {
      margin-right: 1rem;
    }
  }
</style>

<main>
  <div class="left">
    <Portrait {image_url} />
  </div>
  <div class="right">
    <Salutation {greeting} {identify} />
    <Bio>
      Developer currently learning
      <a href="https://www.rust-lang.org/">Rust</a>
      and
      <a href="https://svelte.dev/">Svelte</a>.
      Enjoy exploring
      <a href="https://fs.blog/mental-models/">mental models</a>
      and ways to
      <a href="https://www.youtube.com/watch?v=Tfrrubw7pcE">embrace reality</a>.
      Working as a Director of Application Services while living in Houston, TX.
    </Bio>
    <Links />
  </div>
</main>
