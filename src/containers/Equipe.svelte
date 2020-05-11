<script>
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
    <div class="row">
      {#each integrantes as integrante}
        <div class="col-xs-12 col-md-3">
          <div class="root">
            <img src={integrante.imagem} alt={integrante.nome} />
            <h5>{integrante.nome}</h5>
            <h6>{integrante.cargo}</h6>
            <div class="socials">
              {#if integrante.github}
                <a href={integrante.github} aria-label="Ir para o Github">
                  <i class="fa fa-github" />
                </a>
              {/if}
              {#if integrante.twitter}
                <a href={integrante.twitter} aria-label="Ir para o Twitter">
                  <i class="fa fa-twitter" />
                </a>
              {/if}
              {#if integrante.facebook}
                <a href={integrante.facebook} aria-label="Ir para o Facebook">
                  <i class="fa fa-facebook" />
                </a>
              {/if}
              {#if integrante.linkedin}
                <a href={integrante.linkedin} aria-label="Ir para o Linkedin">
                  <i class="fa fa-linkedin" />
                </a>
              {/if}
              {#if integrante.website}
                <a href={integrante.website} aria-label="Ir para Site Pessoal">
                  <i class="fa fa-link" />
                </a>
              {/if}
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
