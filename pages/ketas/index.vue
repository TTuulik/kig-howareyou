<script setup>
definePageMeta({ layout: "default" });

const options = [
  {
    title: "Õnn",
    options: [
      {
        title: "Rahulolev",
        options: [{ title: "Rahulik" }, { title: "Lõbus" }],
      },
      {
        title: "Uhke",
        options: [{ title: "Rõõmus" }, { title: "Imetlev" }],
      },
    ],
  },
  {
    title: "Elevus",
    options: [
      {
        title: "Optimistlik",
        options: [{ title: "Lootusrikas" }, { title: "Ootusärev" }],
      },
      {
        title: "Erutatud",
        options: [{ title: "Eufooriline" }, { title: "Kergendunud" }],
      },
    ],
  },
  {
    title: "Üllatus",
    options: [
      {
        title: "Segaduses",
        options: [{ title: "Imestunud" }, { title: "Jahmunud" }],
      },
      {
        title: "Overcome",
        options: [{ title: "Liigutatud" }, { title: "Ülekoormatud" }],
      },
    ],
  },
  {
    title: "Hirm",
    options: [
      {
        title: "Ebakindel",
        options: [{ title: "Ärev" }, { title: "Abitu" }],
      },
      {
        title: "Kartlik",
        options: [{ title: "Paanika" }, { title: "Surmahirm" }],
      },
    ],
  },
  {
    title: "Viha",
    options: [
      {
        title: "Ärritunud",
        options: [{ title: "Põlgus" }, { title: "Raev" }],
      },
      {
        title: "Vaenulik",
        options: [{ title: "Vihkamine" }, { title: "Vastumeelsus" }],
      },
    ],
  },
  {
    title: "Kurbus",
    options: [
      {
        title: "Ahastus",
        options: [{ title: "Agoonia" }, { title: "Masendus" }],
      },
      {
        title: "Valu",
        options: [{ title: "Kurvastus" }, { title: "Üksildus" }],
      },
    ],
  },
  {
    title: "Hoolivus",
    options: [
      {
        title: "Murelik",
        options: [{ title: "Vaevatud" }, { title: "Kaastundlik" }],
      },
      {
        title: "Empaatiline",
        options: [{ title: "Kaasaelav" }, { title: "Osavõtlik" }],
      },
    ],
  },
  {
    title: "Armastus",
    options: [
      {
        title: "Iha",
        options: [{ title: "Sentimentaalne" }, { title: "Hellitav" }],
      },
      {
        title: "Kirg",
        options: [{ title: "Romantiline" }, { title: "Igatsus" }],
      },
    ],
  },
];

const options2 = options
  .map((o) => o.options || [{ title: "..." }, { title: "..." }])
  .flat();

const options3 = options
  .map((o) =>
    (o.options || []).map(
      (o2) => o2.options || [{ title: "..." }, { title: "..." }]
    )
  )
  .flat(Infinity);

const selection = $ref({});
const onSelect1 = (sector) =>
  (selection[sector.title] = (selection[sector.title] || 0) + 1);

const rotation = $ref(0);
</script>

<template>
  <div class="grid grid-rows-[1fr_auto] debug h-screen">
    <div class="flex items-center justify-center">
      <TestWheel
        class="w-[180vw] md:w-[60vw] -ml-[90vw] md:ml-0"
        :size="500"
        :style="{
          transform: 'rotate(' + rotation + 'deg)',
        }"
      >
        <circle r="250" />
        <rect x="-100" y="-100" width="200" height="200" fill="white" />
        <rect x="-90" y="-90" width="20" height="20" />
      </TestWheel>
    </div>
    <div class="flex justify-center pb-8">
      <input class="block w-64" type="range" v-model="rotation" max="360" />
    </div>
  </div>
</template>

<style>
.debug {
  @apply border-2 border-blue-500;
}
.debug > * {
  @apply border-2 border-red-500;
}
</style>
