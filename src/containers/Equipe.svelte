<script>
  let integrantes = [1, 2, 3, 4];
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
    <div class="row">
      {#each integrantes as integrante}
        <div class="col-xs-12 col-md-3">
          <div class="root">
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
