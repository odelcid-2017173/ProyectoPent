
<script>
  import Navbar from '../components/navbar/Navbar.svelte';
  import Home from '../components/views/Home.svelte';
  import { Router, Link, Route } from "svelte-routing";

    import { request, gql } from 'graphql-request'

const query = gql`
query {
  posts{
    pages
    rows{
      id
      title
    }

  }
}
`

request('https://blog-backend-blush.vercel.app/graphql', query).then((data) => console.log(data))
</script>

<div>
  <Router>
    <Navbar />
    <Route path="/">
      <Home></Home>
  </Route>
  </Router>
</div>





