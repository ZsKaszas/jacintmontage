<script>
  import icon1 from "../assets/icons/icon1.svg";
  import icon2 from "../assets/icons/icon2.svg";
  import icon3 from "../assets/icons/icon3.svg";

  let cards = [
    {
      icon: { src: icon1, alt: "Maßgefertigte Möbel image" },
      title: "Maßgefertigte Möbel",
      description:
        "Maßgeschneiderte Möbel, ganz nach Ihren Wünschen und Bedürfnissen",
    },
    {
      icon: { src: icon2, alt: "Montage / Demontage image" },
      title: "Montage / Demontage",
      description:
        "Büromöbelmontage Möbelmontage/Demontage Küchenmontage/Demontage",
    },
    {
      icon: { src: icon3, alt: "Transporte image" },
      title: "Transporte",
      description: "Transporte Abholungen von Möbelhäuser",
    },
  ];
</script>

<div class="grid grid-cols-1 sm:grid-cols-3 gap-4">
  {#each cards as card}
    <!-- <img
        src={card.icon.src}
        alt={card.icon.alt}
        class="rounded-lg shadow-lg absolute inset-0 w-full h-full object-cover"
        loading="lazy"
      /> -->
    <div class="h-full bg-[#271d1d] text-[#f5d196] rounded-lg p-4 text-center">
      <img
        src={card.icon.src}
        alt={card.icon.alt}
        class="h-16 mb-4 text-[#f5d196] mx-auto"
        loading="lazy"
      />
      <h3 class="text-2xl font-bold mb-2">{card.title}</h3>
      <p class="text-lg">{card.description}</p>
    </div>
  {/each}
</div>
