<script>
      import { Link } from "svelte-routing";
</script>

<div class="navbarSvelte">
    <nav class="navbar navbar-expand-lg bg-transparent">
      <div class="container-fluid">
        <Link to="/"> 
            <a class="navbar-brand text-light navi" href="#">Your Logo</a>

        </Link>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse flex-row-reverse" id="navbarNavDropdown">
          <ul class="navbar-nav">
            <li class="nav-item">
              <button class="nav-link active text-light  bg-transparent boton1" aria-current="page" href="#">Home</button>
            </li>
            <li class="nav-item">
              <a class="nav-link text-light bg-transparent a1" href="#">About</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-light bg-transparent a1" href="#">Services</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-light bg-transparent a1" href="#">Contact</a>
            </li>
            <li class="a1">
            </li>
          </ul>
        </div>
      </div>
    </nav>
    </div>


<style>
    :global(body){
    background-image: url("https://www.colorhexa.com/29354d.png");
}
.boton1{
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

.a1{
margin-top: 15px;
font-size: 15px;
margin-right: 3rem;
}

.navi{
font-size: 40px;
margin-left: 4rem;
}
</style>

