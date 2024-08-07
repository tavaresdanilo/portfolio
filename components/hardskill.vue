<template>
    <div class="bg-[#FCF5EB] h-screen m-[0] p-[0] box-border flex justify-center items-center flex-col select-none">
    <div class="h-1/3 w-full flex flex-col justify-start items-center p-[3rem] md:p-[6rem]">
      <p class="text-xl md:text-3xl font-semibold text-neutral-700 text-justify">
        Sou um profissional em constante aprendizado. Atráves de projetos pesssoais, tenho aprimorado minhas habilidades ao ganhar conhecimento e experiência em tecnologias, como:
      </p>
    </div>
    <div class="h-full w-full flex flex-col justify-start items-center p-[3rem]">
      <ul class="grid grid-cols-4 md:grid-cols-6 justify-items-center md:gap-[1rem]">
        <li v-for="item in technologies" :key="item" class="flex flex-col items-center gap-[0.5rem] text-neutral-700 my-[1rem]">
          <UIcon :name="`${item.icon}`" class="size-[3rem] md:size-[4rem]" />
          <span class="text-sm md:text-lg font-medium">{{ item.name }}</span>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
const technologies = [
  {
    icon: "mdi:language-html5",
    name: "HTML",
  },
  {
    icon: "mdi:language-css3",
    name: "CSS",
  },
  {
    icon: "mdi:language-javascript",
    name: "JavaScript",
  },
  {
    icon: "mdi:language-php",
    name: "PHP",
  },
  {
    icon: "mdi:vuejs",
    name: "Vue",
  },
  {
    icon: "mdi:laravel",
    name: "Laravel",
  },
  {
    icon: "mdi:tailwind",
    name: "Tailwind",
  },
  {
    icon: "mdi:git",
    name: "Git",
  },
  {
    icon: "mdi:github",
    name: "GitHub",
  },
  {
    icon: "mdi:microsoft-visual-studio-code",
    name: "VS Code",
  },
]
</script>