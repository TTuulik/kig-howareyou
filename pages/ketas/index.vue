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

const showMessage = $ref(true);
</script>

<template>
  <div>
    <div class="grid grid-rows-[1fr_auto] h-screen h-screen-ios">
      <div class="flex items-center justify-center overflow-hidden">
        <TestWheel
          class="w-[180vw] md:w-[60vw] -ml-[90vw] md:ml-0"
          :size="500"
          :style="{
            transform: 'rotate(' + (360 - rotation) + 'deg)',
          }"
        >
          <TestSlices
            @select="onSelect1"
            :selection="selection"
            :options="options"
            :inner="0"
            :outer="80"
          />
          <TestSlices
            @select="onSelect1"
            :selection="selection"
            :options="options2"
            :inner="80"
            :outer="160"
          />
          <TestSlices
            @select="onSelect1"
            :selection="selection"
            :options="options3"
            :inner="160"
            :outer="240"
          />
          <!-- <circle r="250" />
        <rect x="-100" y="-100" width="200" height="200" fill="white" />
        <rect x="-90" y="-90" width="20" height="20" /> -->
        </TestWheel>
      </div>
      <button
        class="fixed top-8 right-8 text-xl font-bold duration-1000 transition"
        :class="[showMessage ? 'opacity-[0.01] -translate-y-4' : 'opacity-30']"
        @click="showMessage = !showMessage"
      >
        ◯
      </button>
      <div
        @click="showMessage = false"
        class="duration-1000 transition fixed top-8 left-8 right-8 md:w-1/3 text-4xl font-bold opacity-70"
        :class="[
          showMessage
            ? 'opacity-80'
            : 'pointer-events-none opacity-0 -translate-y-8',
        ]"
      >
        Su tunded on sinu omad ja nad kõik on väärt mäletamist. Märka ja märgi,
        kuidas sa end tunned.
      </div>
    </div>
    <div class="fixed right-4 bottom-12 left-4 flex justify-center">
      <Slider type="range" v-model="rotation" max="360" />
    </div>
  </div>
</template>

<style>
@supports (-webkit-touch-callout: none) {
  .h-screen-ios {
    height: -webkit-fill-available;
  }
}
</style>
