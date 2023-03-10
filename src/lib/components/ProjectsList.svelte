<script>
  import Project from '$lib/components/Project.svelte'
  import { projects } from '$lib/data/projects.js'
</script>

<div class="projects-list">
  {#each projects as project (project.id)}
    <Project {project} />
  {/each}
</div>