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
      link: "/emotionally/sad",
    },
    {
      title: "Angry",
      fill: "#252C23",
      link: "/emotionally/angry",
    },
    {
      title: "Anxious",
      fill: "#3A4240",
      link: "/emotionally/anxious",
    },
    {
      title: "Mental block",
      fill: "#556D73",
      link: "/emotionally/mentalBlock",
    },
    {
      title: "Confused",
      fill: "#3A4240",
      link: "/emotionally/confused",
    },
  ];

  const onSelect = async (sector) => await navigateTo(sector.link);
</script>
<template>
  <div>
    <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" style="width:100%;"/>
    <div style="padding-left: 50px; padding-top: 5%; height: 100vh;">
      <CircleWheel :options="options" @select="onSelect" />
      <h1 style=" color: #fff; padding-top: 330px; font-size: 40px;">Feelings</h1>
    </div>
    <nuxt-link to="/emotionally" style="position: absolute; left: 20px; bottom: 20px;">
      <img src="/assets/css/back.png" alt="back" class="w-8">
    </nuxt-link>
  </div>
</template>
