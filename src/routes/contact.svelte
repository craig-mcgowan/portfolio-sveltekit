<script>
  import { contactLinks } from "$lib/contactLinks";
</script>

{#each contactLinks as contactLink}

  <div class="flex flex-col items-center">
    <img class="rounded-2xl" src="{contactLink.image}" alt="{contactLink.name}"/>
    <div>
      <h3>{contactLink.name}</h3>
      <p>{contactLink.description}</p>
      <a href="{contactLink.link}">{contactLink.link}</a>
    </div>
  </div>

{/each}