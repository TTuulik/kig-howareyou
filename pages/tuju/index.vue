<script setup>
definePageMeta({ layout: "default" });

const start = [
  {
    title: "",
    fill: "lightblue",
    icon: "/assets/confused-face.svg",
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
    icon: "/assets/smiling-face-with-smiling-eyes.svg",

    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-open-mouth-and-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-heart-shaped-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/smiling-face-with-halo.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/face-with-open-mouth.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/face-with-stuck-out-tongue-and-tightly-closed-eyes.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/face-savouring-delicious-food.svg",
  },
  {
    title: "",
    fill: "#ffaaaa",
    icon: "/assets/grinning-face.svg",
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
