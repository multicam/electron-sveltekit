<script>
    const pages = [['/', 'Home'], ['/page2', 'goto page2'], ['/page3', 'goto page3']]
</script>
<svelte:head>
    <title>Page 1</title>
</svelte:head>

<h1 class="pagetitle">Page 1</h1>
<p>This is the page 1</p>

<div>
    {#each pages as p}
        <a class="button" href='{p[0]}'>{p[1]}</a>
    {/each}
</div>
