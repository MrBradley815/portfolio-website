<script>
  import Icon from '@iconify/svelte'

  export let project
</script>

<div class="project">
  <div class="thumbnail-container">
    <img src="/img/{project.thumbnailUrl}" alt="Space Tourism Website" />
    <div class="overlay"></div>
    <div class="middle">
      <a href="{project.url}" class="btn btn-from-left" target="_blank" rel="noreferrer">VIEW PROJECT</a>
      <a href="{project.github}" class="btn btn-from-right" target="_blank" rel="noreferrer">VIEW CODE</a>
    </div>
  </div>
  <h3>{project.title}</h3>
  <ul class="tech-list">
    {#each project.tech as tech (tech)}
      {#if tech === 'Svelte'}
        <li class="tech-icon svelte">
          <Icon icon="carbon:logo-svelte" />
        </li>
      {:else if tech === 'HTML'}
        <li class="tech-icon html">
          <Icon icon="akar-icons:html-fill" />
        </li>
      {:else if tech === 'CSS'}
        <li class="tech-icon css">
          <Icon icon="akar-icons:css-fill" />
        </li>
      {:else if tech === 'JavaScript'}
        <li class="tech-icon js">
          <Icon icon="akar-icons:javascript-fill" />
        </li>
      {:else if tech === 'Vue'}
        <li class="tech-icon vue">
          <Icon icon="carbon:logo-vue" />
        </li>
      {/if}
    {/each}
  </ul>
</div>