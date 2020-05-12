<script>
  import Grid from "svelte-grid-responsive";
  import knuthShuffle from "knuth-shuffle";
  import Social from "../components/Social.svelte";
  import integrantes from "../data/integrantes.json";
</script>

<style>
  .root {
    color: white;
    padding: 0px 20px;
    text-align: center;
  }

  img {
    width: 100%;
    border-radius: 50%;
    border: 15px solid white;
    margin-bottom: 10px;
  }

  h5 {
    font-size: 25px;
    font-weight: 500;
    margin-bottom: 10px;
  }

  h6 {
    margin-bottom: 20px;
  }
</style>

<section class="context context-invert" id="equipe">
  <h2>Equipe</h2>
  <div class="container">
    <Grid container gutter={12}>
      {#each knuthShuffle.knuthShuffle(integrantes) as integrante}
        <Grid xs={12} md={6} lg={3}>
          <div class="root">
            <img src={integrante.imagem} alt={integrante.nome} />
            <h5>{integrante.nome}</h5>
            <h6>{integrante.cargo}</h6>
            <div class="socials">
              <Social name="github" link={integrante.github} />
              <Social name="twitter" link={integrante.twitter} />
              <Social name="facebook" link={integrante.facebook} />
              <Social name="linkedin" link={integrante.linkedin} />
              <Social name="link" link={integrante.website} />
            </div>
          </div>
        </Grid>
      {/each}
    </Grid>
  </div>
</section>
