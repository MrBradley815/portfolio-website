<script>
  export let skill = {}
</script>

<div class="skill">
  <h2>{skill.title}</h2>

  {#if skill.exp > 1}
    <p>{skill.exp} Years Experience</p>
    {:else}
    <p>{skill.exp} Year Experience</p>
  {/if}
</div>

