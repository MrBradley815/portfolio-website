<script>
  import '$lib/css/footer.css'
  import IconGithub from '$lib/components/icons/IconGithub.svelte'
  import IconLinkedIn from '$lib/components/icons/IconLinkedIn.svelte'
</script>

<footer id="footer">
  <div class="container">
    <div class="footer-inner">
      <div class="footer-left">
        <h1>Contact</h1>
        <p>I would love to hear about your project and how I could help. Please fill in the form, and I'll get back to you as soon as possible.</p>
      </div>
      <div class="footer-right">
        <form action="#" method="POST" autocomplete="off">
          <input type="text" name="Name" placeholder="NAME" />
          <input type="email" name="Email" placeholder="EMAIL" />
          <textarea name="Message" placeholder="MESSAGE"></textarea>
          <button type="submit" class="btn btn-submit">SEND MESSAGE</button>
        </form>
      </div>
    </div>
    <hr>
    <div class="footer-bottom">
      <div class="logo">bradproctor</div>
      <ul class="social">
        <li><a href="https://github.com/MrBradley815" target="_blank" rel="noreferrer"><IconGithub /></a></li>
        <li><a href="https://www.linkedin.com/in/brad-proctor-91b61b132/" target="_blank" rel="noreferrer"><IconLinkedIn /></a></li>
      </ul>
    </div>
  </div>
</footer>