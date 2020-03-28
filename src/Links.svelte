<script>
  import Icon from "svelte-awesome";
  import { github, twitter, linkedin } from "svelte-awesome/icons";
  let links = [
    { name: github, url: "https://github.com/bradyjoslin" },
    { name: twitter, url: "https://twitter.com/bradyj" },
    { name: linkedin, url: "https://linkedin.com/in/bradyjoslin" }
  ];
</script>

<style>
  a {
    color: #eee;
    margin: 0.25rem;
  }

  a:hover {
    color: #333;
  }
</style>

<div class="links">
  {#each links as { name, url }}
    <a rel="me" href={url} title={Object.getOwnPropertyNames(name)}>
      <Icon data={name} scale="2" />
    </a>
  {/each}
</div>
