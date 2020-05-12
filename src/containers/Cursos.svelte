<script>
  import Grid from "svelte-grid-responsive";
  import cursos from "../data/cursos.json";
</script>

<div class="container">
  <section class="context" id="cursos">
    <h2>Cursos</h2>
    <Grid container gutter={12}>
      {#each cursos as curso}
        <Grid xs={12} md={6} lg={4}>
          <div class="card">
            <iframe
              title={`Playlist do curso '${curso.titulo}'`}
              type="text/html"
              width="100%"
              height="250"
              src={curso.embedYoutube}
              frameborder="0"
              allow="accelerometer; autoplay; encrypted-media; gyroscope;
              picture-in-picture"
              allowfullscreen />
            <div class="card-body">
              <h5 class="card-title">{curso.titulo}</h5>
              <p class="card-text">{curso.descricao}</p>
              {#if curso.github}
                <a href={curso.github} class="btn btn-primary">
                  Acessar o GitHub
                </a>
              {/if}
            </div>
          </div>
        </Grid>
      {/each}
    </Grid>
  </section>
</div>
