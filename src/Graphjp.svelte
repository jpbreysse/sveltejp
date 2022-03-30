
<script>



import { initClient } from "@urql/svelte";
  
    initClient({
      url: "https://api.blaqkube.io/"
    });


  import { operationStore, query } from '@urql/svelte';


  const todos = operationStore(
  query {
	  instances("connection":"","namespace":"")
        {name
        }
  }
  );

  $from: Int!, $limit: Int!




  query(todos);
</script>

{#if $todos.fetching}
<p>Loading...</p>
{:else if $todos.error}
<p>Oh no... {$todos.error.message}</p>
{:else}
<ul>
  {#each $todos.data.todos as todo}
  <li>{todo.title}</li>
  {/each}
</ul>
{/if}