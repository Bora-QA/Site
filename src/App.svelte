<script>
  import Social from "./components/Social.svelte";

  import CursosContainer from "./containers/Cursos.svelte";
  import EquipeContainer from "./containers/Equipe.svelte";
  import SobreContainer from "./containers/Sobre.svelte";
</script>

<style>
  header {
    background-color: #675cf3;
    min-height: 400px;
    padding: 50px 0px;
    margin: auto;
    text-align: center;
    color: white;
    background: radial-gradient(#675cf3 20%, #4537f0);
  }

  header img {
    width: 200px;
    height: auto;
  }

  header h1 {
    font-weight: 600;
    margin-top: 20px;
    font-size: 80px;
  }

  header h4 {
    margin-bottom: 40px;
  }

  nav {
    box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14),
      0 3px 1px -2px rgba(0, 0, 0, 0.12), 0 1px 5px 0 rgba(0, 0, 0, 0.2);
  }

  nav img {
    height: 40px;
  }

  footer {
    padding: 15px;
    text-align: center;
    box-shadow: 0 -2px 2px 0 rgba(0, 0, 0, 0.14),
      0 -3px 1px -2px rgba(0, 0, 0, 0.12), 0 -1px 5px 0 rgba(0, 0, 0, 0.2);
  }
</style>

<nav class="navbar navbar-expand-lg navbar-light bg-light sticky-top">
  <a class="navbar-brand" href="/">
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
        <a
          class="nav-link"
          href="https://github.com/Bora-QA/Sobre/blob/master/CODE_OF_CONDUCT.md">
          Código de Conduta
        </a>
      </li>
    </ul>
  </div>
</nav>
<header>
  <img src="./assets/logo-border.png" alt="Bora QA" />
  <h1>Bora QA</h1>
  <h4>Compartilhando conhecimento e andando juntos</h4>
  <div class="socials">
    <Social name="github" link="http://github.com/bora-QA" />
    <Social name="twitter" link="https://www.youtube.com/" />
  </div>
</header>

<CursosContainer />
<EquipeContainer />
<SobreContainer />

<footer>Copyright © 2020 Bora QA</footer>
