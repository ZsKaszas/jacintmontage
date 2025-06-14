<script>
  let { animate = false } = $props();
</script>

<a
  href="mailto:jacintmontage@gmail.com"
  aria-label="Email address"
  class={animate ? " animate-pulse" : ""}
  ><span class="icon-[line-md--email]"></span>
</a>
