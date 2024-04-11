<template>
  <div class="flex">
    <div class="light h-screen w-1/2 p-4 flex items-center justify-center flex-col gap-8">
      <h2 class="text-2xl font-bold">Light mode</h2>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti adipisci exercitationem
        cumque possimus at ex dolores. Distinctio, ullam placeat dicta non eius quo veniam corporis
        cupiditate possimus sequi neque? In?
      </p>
    </div>
    <div class="dark h-screen w-1/2 p-4 flex items-center justify-center flex-col gap-8">
      <h2 class="text-2xl font-bold">Dark mode</h2>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti adipisci exercitationem
        cumque possimus at ex dolores. Distinctio, ullam placeat dicta non eius quo veniam corporis
        cupiditate possimus sequi neque? In?
      </p>
    </div>
  </div>
</template>

<style scoped>
.dark {
  --bkg: var(--bkg-dark);
  --text: var(--text-dark);
  background-color: hsl(var(--bkg));
  color: hsl(var(--text));
}

.light {
  --bkg: var(--bkg-light);
  --text: var(--text-light);
  background-color: hsl(var(--bkg));
  color: hsl(var(--text));
}
</style>
