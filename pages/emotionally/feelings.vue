<script setup>
definePageMeta({ layout: "emotionally" });
const options = [
  {
    title: "Tired",
    fill: "#2F4E3E",
    link: "/emotionally/tired",
  },
  {
    title: "Sad",
    fill: "#556D73",
    link: "/emotionally/tired",
  },
  {
    title: "Angry",
    fill: "#252C23",
    link: "/emotionally/tired",
  },
  {
    title: "Anxious",
    fill: "#3A4240",
    link: "/emotionally/tired",
  },
  {
    title: "Mental block",
    fill: "#556D73",
    link: "/emotionally/tired",
  },
  {
    title: "Confused",
    fill: "#3A4240",
    link: "/emotionally/tired",
  },
];

const onSelect = async (sector) => await navigateTo(sector.link);
</script>
<template>
  <div>
    <img
      src="/assets/css/Background.png"
      class="h-screen object-cover fixed -z-10"
    />
    <div style="padding-left: 50px; padding-top: 130px; word-wrap: break-word">
      <CircleWheel :options="options" @select="onSelect" />
    </div>
    <h1
      style="
        color: #fff;
        padding-top: 245px;
        padding-left: 20px;
        font-size: 40px;
      "
    >
      Feelings
    </h1>
  </div>
</template>
