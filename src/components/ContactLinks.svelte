<script>
  import {contactLinks} from "$lib/contactLinks";
</script>

<div class="flex w-max">

  {#each contactLinks as {site, url, icon} }
  
  <div class = "m-2">
    <a href={url} target=_blank >
      <div class= "h-16 my-2 p-2 hover:h-18 hover:text-teal-400" >
        <svelte:component this={icon} class="h-10 hover:h-18"/>
      </div>

    </a>
  </div>
  
  {/each}
</div>