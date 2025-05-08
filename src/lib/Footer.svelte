<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  import Logo from "./Logo.svelte";
</script>

<footer class="bg-[#271d1d] text-[#f5d196]">
  <SectionWrapper>
    <div
      class="grid grid-cols-2 sm:grid-cols-3 justify-between gap-4 items-center text-center"
    >
      <div
        class="h-20 col-span-2 sm:col-span-1 flex justify-center sm:justify-start items-center"
      >
        <Logo />
      </div>
      <div class="text-2xl">Seit 2024</div>
      <div class="flex gap-8 text-2xl justify-center sm:justify-end">
        <a href="tel:+491627732136" aria-label="Phone number">
          <span class="icon-[line-md--phone]"></span>
        </a>
        <a href="mailto:jacintmontage@gmail.com" aria-label="Email address"
          ><span class="icon-[line-md--email]"></span>
        </a>
        <a
          href="https://facebook.com/profile.php?id=61555968216358"
          target="_blank"
          aria-label="Facebook profile"
          ><span class="icon-[line-md--facebook]"></span>
        </a>
        <a
          href="https://instagram.com/jacintmontage/"
          target="_blank"
          aria-label="Instagram profile"
          ><span class="icon-[line-md--instagram]"></span>
        </a>
      </div>
    </div>
  </SectionWrapper>
</footer>
