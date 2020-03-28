<script>
  import Salutation from "./Salutation.svelte";
  import Portrait from "./Portrait.svelte";
  import Bio from "./Bio.svelte";
  import Links from "./Links.svelte";
</script>

<style>
  :global(body) {
    color: #eee;
    background-color: #6200ee;
    font-family: "Roboto", "Helvetica Neue", "Segoe UI", Helvetica, Arial,
      sans-serif;
    font-size: 16px;
    overflow-y: auto;
  }

  .column {
    flex: 1;
  }

  main {
    display: flex;
    margin-top: 20vh;
  }

  main .right {
    margin-right: 2rem;
  }

  @media screen and (max-width: 992px) {
    main {
      flex-direction: column;
      margin: 0;
    }

    main .column.left {
      text-align: center;
    }

    main .portrait {
      margin: 0;
    }

    main .footer {
      margin: 0;
    }
  }

  main .footer {
    display: flex;
    margin-top: 1rem;
    font-size: 1.5rem;
  }

  @media screen and (max-width: 992px) {
    main .footer {
      flex-direction: column;
    }
  }
</style>

<main>
  <div class="column left">
    <span class="portrait">
      <Portrait />
    </span>
  </div>
  <div class="column right">
    <Salutation />
    <Bio />
    <div class="footer">
      <Links />
    </div>
  </div>
</main>
