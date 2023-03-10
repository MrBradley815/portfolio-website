<script>
  import '$lib/css/main.css'
  import SkillsList from '$lib/components/SkillsList.svelte'
  import ProjectsList from '$lib/components/ProjectsList.svelte'
  import bradPortraitLg from '$lib/images/placeholder.png'
  import bradPortraitMd from '$lib/images/placeholder-tablet.png'
  import bradPortraitSm from '$lib/images/placeholder-mobile.png'
  import circleImg from '$lib/images/pattern-circle.svg'
  import ringsImg from '$lib/images/pattern-rings.svg'
</script>

<main>
  <div class="container">
    <section id="hero">
      <h1>Nice to meet you! I'm <span class="name">Brad Proctor</span>.</h1>
      <p>Based in Texas, I'm a front-end developer passionate about building accessible web apps that users love.</p>
      <a href="#footer" class="btn">CONTACT ME</a>
      <picture>
        <source srcset="{bradPortraitLg}" media="(min-width: 1175px)">
        <source srcset="{bradPortraitMd}" media="(min-width: 701px)">
        <img src="{bradPortraitSm}" class="portrait" alt="Portrait of Brad" />
      </picture>
      <img src="{circleImg}" class="circle" alt="Circle" />
      <img src="{ringsImg}" class="rings" alt="Rings" />
    </section>

    <hr>

    <section id="skills">
      <SkillsList />
    </section>

    <section id="projects">
      <div class="projects-header">
        <h1>Projects</h1>
        <a href="#footer" class="btn">CONTACT ME</a>
      </div>
      <ProjectsList />
    </section>
  </div>
</main>