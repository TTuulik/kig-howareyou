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
           options: [{ title: "Vihkamine"}, { title: "Vastumeelsus"}],
        },
      ],
  },
  {
    title: "Kurbus",
    options: [
      {
        title: "Ahastus",
         options: [{ title: "Agoonia" }, { title: "Masendus"}],
         },
         {
          title: "Valu",
           options: [{ title: "Kurvastus" }, { title: "Üksildus"}],
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
           options: [{ title: "Kaasaelav" }, { title: "Osavõtlik"}],
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
