<script>
  export let image_url;
</script>

<style>
  img {
    border-radius: 50%;
    border: 10px solid #eee;
    width: 100%;
    max-width: 300px;
    max-height: 300px;
  }

  @media screen and (max-width: 800px) {
    img {
      border-radius: 50%;
      border: 7.5px solid #eee;
      width: 100%;
      max-width: 250px;
      max-height: 250px;
    }
  }
</style>

<img src={image_url} alt="Portrait" />
