<script>
  import Icon from "svelte-awesome";
  export let links = [];
</script>

<style>
  a {
    margin: 0.25rem;
    text-decoration: none;
  }
</style>

<div class="links">
  {#each links as { name, url }}
    <a rel="me" href={url} title={Object.getOwnPropertyNames(name)}>
      <Icon data={name} scale="2" />
    </a>
  {/each}
</div>
