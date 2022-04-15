<script>
  import { projects } from "$lib/projects";

</script>

<h1>Projects</h1>
{#each projects as project }

  <div class="flex flex-col items-center">
    <img class="rounded-2xl" src="{project.image}" alt="{project.name}"/>
    <div>
      <h3>{project.name}</h3>
      <p>{project.description}</p>
      <a href="{project.link}">{project.link}</a>
    </div>
  </div>

{/each}