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
  <div class="flex items-center justify-center h-full">
    <!-- <div class="fixed top-32 left-12 text-6xl font-bold opacity-80">
      Feelings are normal. They need to be illuminated. Here is how you can do
      it. Every day, mark an emotion. Or two. Or three.
    </div> -->
    <div class="p-8">
      <TestWheel
        :size="800"
        :style="{
          transform:
            'translate(-50px,220px) rotate(' + rotation + 'deg) scale(1.3)',
        }"
      >
        <TestSlices
          @select="onSelect1"
          :selection="selection"
          :options="options"
          :inner="0"
          :outer="120"
        />
        <TestSlices
          @select="onSelect1"
          :selection="selection"
          :options="options2"
          :inner="120"
          :outer="220"
        />
        <TestSlices
          @select="onSelect1"
          :selection="selection"
          :options="options3"
          :inner="220"
          :outer="350"
        />
      </TestWheel>
    </div>
    <div class="fixed top-8 left-8">
      <input type="range" v-model.number="rotation" class="w-64" max="360" />
    </div>
  </div>
</template>
