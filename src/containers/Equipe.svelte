<script>
  let integrantes = [1, 2, 3, 4];
</script>

<section class="context context-invert" id="equipe">
  <h2>Equipe</h2>
  <div class="container">
    <div class="row">
      {#each integrantes as integrante}
        <div class="col-xs-12 col-md-3">
          <div class="user">
            <img src="./assets/user.png" alt="Rosto do Integrante sorrindo" />
            <h5>Integrante</h5>
            <h6>QA</h6>
            <div class="socials">
              <a
                href="https://www.facebook.com/"
                aria-label="Ir para o Facebook">
                <i class="fa fa-facebook" />
              </a>
              <a
                href="https://twitter.com/andrelmlins"
                aria-label="Ir para o Twitter">
                <i class="fa fa-twitter" />
              </a>
              <a href="http://github.com/" aria-label="Ir para o Github">
                <i class="fa fa-github" />
              </a>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
