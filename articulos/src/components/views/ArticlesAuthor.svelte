<script context="module">
    import { request, gql } from 'graphql-request'
    
    const query = gql`
    query {
  posts{
    pages
    rows{
      author{
        name
      }
      title
    }

  }
}`
    
    request('https://blog-backend-blush.vercel.app/graphql', query).then((data) => console.log(data))
    </script>
    
    <div class="title text-light">
       Articulos Por Autor<br>
      Solo  se puede ver por consola.
    </div>
    
    <style>
          .title{
            font-size: 3vw;
            font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif ;
            margin-left: 26vw;
            margin-top: 10vw;
            margin-bottom: 10vw;
        }
    </style>