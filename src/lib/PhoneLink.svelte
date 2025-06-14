<script>
  let { animate = false } = $props();
</script>

<a
  href="tel:+491627732136"
  aria-label="Telefonnummer"
  class={animate ? " animate-pulse" : ""}
>
  <span class="icon-[line-md--phone]"></span>
</a>
