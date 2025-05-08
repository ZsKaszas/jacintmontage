<script>
  import project1 from "../assets/project-1.jpg";
  import project2 from "../assets/project-2.jpg";
  import project3 from "../assets/project-3.jpg";
  import project4 from "../assets/project-4.jpg";
  import project5 from "../assets/project-5.jpg";
  import project6 from "../assets/project-6.jpg";
  import project7 from "../assets/project-7.jpg";
  import project8 from "../assets/project-8.jpg";
  import project9 from "../assets/project-9.jpg";
  import project10 from "../assets/project-10.jpg";
  import project11 from "../assets/project-11.jpg";
  import project12 from "../assets/project-12.jpg";
  import project13 from "../assets/project-13.jpg";
  import project14 from "../assets/project-14.jpg";
  import project15 from "../assets/project-15.jpg";
  import project16 from "../assets/project-16.jpg";
  import project17 from "../assets/project-17.jpg";

  let images = [
    { src: project1, alt: "Project 1" },
    { src: project2, alt: "Project 2" },
    { src: project3, alt: "Project 3" },
    { src: project4, alt: "Project 4" },
    { src: project5, alt: "Project 5" },
    { src: project6, alt: "Project 6" },
    { src: project7, alt: "Project 7" },
    { src: project8, alt: "Project 8" },
    { src: project9, alt: "Project 9" },
    { src: project10, alt: "Project 10" },
    { src: project11, alt: "Project 11" },
    { src: project12, alt: "Project 12" },
    { src: project14, alt: "Project 14" },
    { src: project13, alt: "Project 13" },
    { src: project15, alt: "Project 15" },
    { src: project16, alt: "Project 16" },
    { src: project17, alt: "Project 17" },
  ];
</script>

<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
  {#each images as image}
    <div class="h-94 md:h-80 lg:h-96 overflow-hidden relative">
      <img
        src={image.src}
        alt={image.alt}
        class="rounded-lg shadow-lg absolute inset-0 w-full h-full object-cover"
        loading="lazy"
      />
    </div>
  {/each}
</div>
