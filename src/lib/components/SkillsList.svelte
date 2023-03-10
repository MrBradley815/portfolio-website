<script>
  import Skill from '$lib/components/Skill.svelte'
  import { skills } from '$lib/data/skills.js'
</script>

{#each skills as skill (skill.id)}
  <Skill {skill} />
{/each}