
<script >
  import Navbar from '../components/navbar/Navbar.svelte';
  import Home from '../components/views/Home.svelte';
  import About from '../components/views/About.svelte';
  import Services from '../components/views/Services.svelte';
  import Contact from '../components/views/contact.svelte';
  import Articles from '../components/views/Articles.svelte';
  import ArticlesCategory from '../components/views/ArticlesCategory.svelte';
  import ArticlesAuthor from '../components/views/ArticlesAuthor.svelte';
  import { Router, Link, Route } from "svelte-routing";

</script>

<div>
  <Router>
    <Navbar />
    <Route path="/">
      <Home></Home>
  </Route>
  <Route path="/about">
    <About></About>
</Route>
<Route path="/services">
  <Services></Services>
</Route>
<Route path="/contact" >
  <Contact></Contact>
</Route>
<Route path="/articles" >
  <Articles></Articles>
</Route>
<Route path="/articlesCategory" >
  <ArticlesCategory></ArticlesCategory>
</Route>
<Route path="/articlesAuthor" >
  <ArticlesAuthor></ArticlesAuthor>
</Route>
  </Router>
</div>





