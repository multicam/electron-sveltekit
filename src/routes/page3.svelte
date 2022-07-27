<script>
  const pages = [['/', 'Home'], ['/page1', 'goto page1'], ['/page2', 'goto page2']]
</script>
<svelte:head>
  <title>Page 1</title>
</svelte:head>

<h1 class="pagetitle">Page 3</h1>
<p>This is the page 3</p>

<div>
    {#each pages as p}
        <a class="button" href='{p[0]}'>{p[1]}</a>
    {/each}
</div>
