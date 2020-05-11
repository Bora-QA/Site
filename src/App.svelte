<script>
  import CursosContainer from "./containers/Cursos.svelte";
  import EquipeContainer from "./containers/Equipe.svelte";
  import SobreContainer from "./containers/Sobre.svelte";
</script>

<nav class="navbar navbar-expand-lg navbar-light bg-light sticky-top">
  <a class="navbar-brand" href="#">
    <img src="./assets/logo-header.png" alt="Bora QA" />
  </a>
  <button
    class="navbar-toggler"
    type="button"
    data-toggle="collapse"
    data-target="#navbarNav"
    aria-controls="navbarNav"
    aria-expanded="false"
    aria-label="Toggle navigation">
    <span class="navbar-toggler-icon" />
  </button>
  <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item active font-weight-bold">
        <a class="nav-link" href="#cursos">Cursos</a>
      </li>
      <li class="nav-item active font-weight-bold">
        <a class="nav-link" href="#equipe">Equipe</a>
      </li>
      <li class="nav-item active font-weight-bold">
        <a class="nav-link" href="#quem-somos">Quem somos</a>
      </li>
      <li class="nav-item active font-weight-bold">
        <a class="nav-link" href="#">Código de Conduta</a>
      </li>
    </ul>
  </div>
</nav>
<header>
  <img src="./assets/logo-border.png" alt="Bora QA" />
  <h1>Bora QA</h1>
  <h4>Compartilhando conhecimento e andando juntos</h4>
  <div class="socials">
    <a href="#" class="fa fa-github" aria-label="Ir para o Github" />
    <a href="#" class="fa fa-youtube" aria-label="Ir para o canal no Youtube" />
  </div>
</header>

<CursosContainer />
<EquipeContainer />
<SobreContainer />

<footer>Copyright © 2020 Bora QA</footer>
