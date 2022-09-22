<script>
  import { Link } from "svelte-routing";
</script>

<div class="navbarSvelte">
  <nav class="navbar navbar-expand-lg bg-transparent">
    <div class="container-fluid">
      <Link to="/" style={"text-decoration: none"}>
        <a class="navbar-brand text-light navi" href="#home">Your Logo</a>
      </Link>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNavDropdown"
        aria-controls="navbarNavDropdown"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon" />
      </button>
      <div
        class="collapse navbar-collapse flex-row-reverse"
        id="navbarNavDropdown"
      >
        <ul class="navbar-nav">
          <li class="nav-item">
            <Link to="/" style={"text-decoration: none"}
              ><button
                class="nav-link active text-light  bg-transparent boton1"
                aria-current="page"
                href="#home">Home</button
              ></Link
            >
            >
          </li>
          <li class="nav-item">
            <Link to="/about" style={"text-decoration: none"}
              ><a class="nav-link text-light bg-transparent a1" href="#about"
                >About</a
              ></Link
            >
          </li>
          <li class="nav-item">
            <Link to="/services" style={"text-decoration: none"}
              ><a class="nav-link text-light bg-transparent a1" href="#services"
                >Services</a
              ></Link
            >
          </li>
          <li class="nav-item">
            <Link to="/contact" style={"text-decoration: none"}
              ><a class="nav-link text-light bg-transparent a1" href="#contac"
                >Contact</a
              ></Link
            >
          </li>
          <li class="a1">
            <div class="dropdown">
              <a
                class="btn dropdown-toggle bg-transparen text-light"
                role="button"
                id="dropdownMenuLink"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                Articulos
              </a>

              <ul class="dropdown-menu" aria-labelledby="dropdownMenuLink">
                <li>
                  <Link to="/articles" style={"text-decoration: none"}
                    ><a class="dropdown-item" href="#categoria">Articulos</a
                    ></Link
                >
                </li>
                <li>
                  <Link to="/articlesCategory" style={"text-decoration: none"}
                    ><a class="dropdown-item" href="#categoria">Categoria</a
                    ></Link
                  >
                </li>
                <li>
                  <Link to="/articlesAuthor" style={"text-decoration: none"}
                    ><a class="dropdown-item" href="#categoria">Autor</a
                    ></Link
                  >
                </li>
              </ul>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</div>

<style>
  :global(body) {
    background-image: url("https://www.colorhexa.com/29354d.png");
  }
  .boton1 {
    background: transparent;
    color: #fff;
    margin: 15px;
    border: 3px solid #fff;
    padding: 5px;
    padding-left: 15px;
    padding-right: 15px;
    border-radius: 50px 50px 50px 50px;
    font-size: 15px;
    margin-right: 3rem;
  }

  .a1 {
    margin-top: 15px;
    font-size: 15px;
    margin-right: 3rem;
  }

  .navi {
    font-size: 40px;
    margin-left: 4rem;
    text-decoration: none;
  }
</style>
