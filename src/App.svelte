<script>
  const themes = [
    "light",
    "dark",
    "cupcake",
    "bumblebee",
    "emerald",
    "corporate",
    "synthwave",
    "retro",
    "cyberpunk",
    "valentine",
    "halloween",
    "garden",
    "forest",
    "aqua",
    "lofi",
    "pastel",
    "fantasy",
    "wireframe",
    "black",
    "luxury",
    "dracula",
    "cmyk",
    "autumn",
    "business",
    "acid",
    "lemonade",
    "night",
    "coffee",
    "winter",
  ];
  let theme;
  const getRandomTheme = () => {
    let rand = Math.random() * (themes.length + 1);
    console.log(rand);
    theme = themes[Math.floor(rand)]
  };
  getRandomTheme();
</script>

<main
  class="w-full min-h-screen flex relative justify-center items-center"
  data-theme={theme}>
  <div class=" bg-secondary rounded-md p-5 flex flex-col gap-3">
    <h1 class=" text-5xl">Hello world!</h1>
    <button class="btn btn-active btn-accent" on:click={getRandomTheme}>Change theme</button>
  </div>
</main>

<style>
</style>
