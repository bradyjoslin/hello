<script>
  import { github, twitter, linkedin } from "svelte-awesome/icons";
  import Salutation from "./components/Salutation.svelte";
  import Portrait from "./components/Portrait.svelte";
  import My_Bio from "./My_Bio.svelte";
  import Links from "./components/Links.svelte";

  let greeting = "Hello!";
  let identify = "I am Brady.";
  let image_url = "./static/images/portrait.jpg";
  let links = [
    { name: github, url: "https://github.com/bradyjoslin" },
    { name: twitter, url: "https://twitter.com/bradyj" },
    { name: linkedin, url: "https://linkedin.com/in/bradyjoslin" }
  ];
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
    <My_Bio />
    <Links {links} />
  </div>
</main>
