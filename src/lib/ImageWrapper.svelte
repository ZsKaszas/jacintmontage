<script>
  import { fade } from "svelte/transition";

  let { image } = $props();
</script>

<div
  class="h-94 md:h-80 lg:h-96 overflow-hidden relative"
  transition:fade={{ delay: 1000 }}
>
  <img
    src={image.src}
    alt={image.alt}
    class="rounded-lg shadow-lg absolute inset-0 w-full h-full object-cover"
    loading="lazy"
  />
</div>
