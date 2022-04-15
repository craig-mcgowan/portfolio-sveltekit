<script>
  import { goto } from "$app/navigation";
  import { contactLinks } from "$lib/contactLinks";
</script>

{#each contactLinks as {site, url, icon} }

  <div class="flex flex-col items-center">
    <a href={url} target=_blank >
      <div class= "h-16 flex-grow-0 my-2  p-2 rounded-2xl min-w-fit duration-200 ease-linear transition-all" >
        <svelte:component this={icon} class="h-10"/>
      </div>
      <div>
        <h3>{site}</h3>
      </div>
    </a>
  </div>

{/each}