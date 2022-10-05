<script setup>
definePageMeta({ layout: "default" });

const start = [
  {
    title: "",
    fill: "red",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "yellow",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
];

const up = [
{

title: "",
fill: "#ffaaaa",
icon: "/assets/smiling-face-with-smiling-eyes",

title: "",
fill: "#ffaaaa",
icon: "/assets/smiling-face-with-open-mouth-and-smiling-eyesg",
},
{

title: "",
fill: "#ffaaaa",
icon: "/assets/smiling-face-with-heart-shaped-eyes",
},
{
title: "",
fill: "#ffaaaa",
icon: "/assets/smiling-face-with-halo",
},
{
title: "",
fill: "#ffaaaa",
icon: "/assets/face-with-open-mouth",
},
{
title: "",
fill: "#ffaaaa",
icon: "/assets/face-with-stuck-out-tongue-and-tightly-closed-eyes",
},
{
title: "",
fill: "#ffaaaa",
icon: "/assets/face-savouring-delicious-food",
},
{
title: "",
fill: "#ffaaaa",
icon: "/assets/grinning-face",
},

];

const up2 = [
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
];

const down = [
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/angry-face.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/confounded-face.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/confused-face.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/disappointed-but-relieved-face.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/expressionless-face.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/loudly-crying-face.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/tired-face.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
];

const down2 = [
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
];
</script>

<template>
  <div class="">
    <div>
      <div>Start</div>
      <TestWheel>
        <TestSlices
          :options="start"
          :inner="50"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
      <div>Up</div>
      <TestWheel>
        <TestSlices
          :options="up"
          :inner="50"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
      <div>Up2</div>
      <TestWheel>
        <TestSlices
          :options="up2"
          :inner="50"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
      <div>Down</div>
      <TestWheel>
        <TestSlices
          :options="down"
          :inner="50"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
      <div>Down2</div>
      <TestWheel>
        <TestSlices
          :options="down2"
          :inner="50"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
    </div>
  </div>
</template>
