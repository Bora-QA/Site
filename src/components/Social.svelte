<script>
  export let name;
  export let link;
</script>

<style>
  .fa {
    font-size: 25px;
    width: 50px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    border-radius: 50%;
    border: 2px solid white;
    background-color: transparent;
    color: white;
    transition: 0.2s all;
  }

  a:hover {
    text-decoration: none;
  }

  a {
    margin-right: 15px;
  }

  a:last-child {
    margin-right: 0px;
  }

  .fa:hover {
    text-decoration: none;
    border-color: white;
    background-color: white;
    color: #675cf3;
  }
</style>

{#if link}
  <a href={link} aria-label={`Ir para ${name}`} target="_blank">
    <i class={`fa fa-${name}`} />
  </a>
{/if}
