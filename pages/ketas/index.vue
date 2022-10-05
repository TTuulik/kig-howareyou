<script setup>
definePageMeta({ layout: "default" });

const options = [
  {
    title: "Õnn",
    fill: "#ffaaaa",
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
    fill: "yellow",
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
    fill: "red",
    options: [{ title: "Segaduses" }, { title: "Kergendunud" }],
  },
  {
    title: "Mure",
    fill: "green",
    options: [{ title: "Ebakindel" }, { title: "Kartlik" }],
  },
  {
    title: "Viha",
    fill: "#ffaaaa",
    options: [{ title: "Ärritunud" }, { title: "Vaenulik" }],
  },
  {
    title: "Kurbus",
    fill: "yellow",
    options: [{ title: "Ahastus" }, { title: "Valu" }],
  },
  {
    title: "Hoolivus",
    fill: "red",
    options: [{ title: "Murelik" }, { title: "Empaatiline" }],
  },
  {
    title: "Armastus",
    fill: "green",
    options: [{ title: "Iha" }, { title: "Kirglik" }],
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

const selected1 = $ref();
const selected2 = $ref();
const selected3 = $ref();
const onSelect1 = (sector) => (selected1 = sector);
const onSelect2 = (sector) => (selected2 = sector);
const onSelect3 = (sector) => (selected3 = sector);
</script>

<template>
  <div class="flex items-center justify-center h-full">
    <div class="p-8">
      <TestWheel :size="800">
        <TestSlices
          @select="onSelect1"
          :options="options"
          :inner="0"
          :outer="120"
        />
        <TestSlices
          @select="onSelect2"
          :options="options2"
          :inner="120"
          :outer="220"
          :class="[selected1 ? '' : '']"
        />
        <TestSlices
          @select="onSelect3"
          :options="options3"
          :inner="220"
          :outer="350"
          :class="[selected2 ? '' : '']"
        />
      </TestWheel>
    </div>
  </div>
</template>
