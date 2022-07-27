<script>
  const pages = [['/page1', 'goto page1'], ['/page2', 'goto page2'], ['/page3', 'goto page3']]
</script>

<svelte:head>
  <title>Svelte Template</title>
</svelte:head>

<main>
  <h1 class="text-primary">Hello world!</h1>
</main>

<div>
    {#each pages as p}
        <a class="button" href='{p[0]}'>{p[1]}</a>
    {/each}
</div>
