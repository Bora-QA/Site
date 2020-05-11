<script>
  let cursos = [1, 2, 3];
</script>

<div class="container">
  <section class="context" id="cursos">
    <h2>Cursos</h2>
    <div class="row">
      {#each cursos as curso}
        <div class="col-xs-12 col-md-4 curso">
          <div class="card">
            <iframe
              title="Playlist do curso 'Como pensar em qualidade?'"
              type="text/html"
              width="100%"
              height="250"
              src="https://www.youtube.com/embed/lcKo-ycLDNw?list=PLx4x_zx8csUj3IbPQ4_X5jis_SkCol3eC"
              frameborder="0"
              allow="accelerometer; autoplay; encrypted-media; gyroscope;
              picture-in-picture"
              allowfullscreen />
            <div class="card-body">
              <h5 class="card-title">Como pensar em qualidade?</h5>
              <p class="card-text">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry. Lorem Ipsum has been the industry's standard dummy
                text ever since the 1500s.
              </p>
              <a href="https://github.com/" class="btn btn-primary">
                Acessar o github
              </a>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </section>
</div>
