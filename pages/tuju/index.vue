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
    fill: "#FFCC80",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    title: "",
    fill: "#FDBA74",
    icon: "/assets/smiling-face-with-heart-shaped-eyes.svg",
  },
  {
    title: "",
    fill: "#FDE68A",
    icon: "/assets/smiling-face-with-halo.svg",
  },
  {
    title: "tere",
    fill: "#FECDD3",
    icon: "/assets/face-with-open-mouth.svg",
  },
  {
    title: "",
    fill: "#FFBB89",
    icon: "/assets/face-with-stuck-out-tongue-and-tightly-closed-eyes.svg",
  },
  {
    title: "",
    fill: "#FED7AA",
    icon: "/assets/face-savouring-delicious-food.svg",
  },
  {
    title: "",
    fill: "#FECACA",
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
    fill: "purple",
    icon: "/assets/angry-face.svg",
  },
  {
    title: "",
    fill: "lightpurple",
    icon: "/assets/confounded-face.svg",
  },
  {
    title: "",
    fill: "skyblue",
    icon: "/assets/confused-face.svg",
  },
  {
    title: "",
    fill: "#9FA1A1",
    icon: "/assets/disappointed-but-relieved-face.svg",
  },
  {
    title: "",
    fill: "#faebecc",
    icon: "/assets/expressionless-face.svg",
  },
  {
    title: "",
    fill: "#83ABC1",
    icon: "/assets/loudly-crying-face.svg",
  },
  {
    title: "",
    fill: "#lightpurple",
    icon: "/assets/tired-face.svg",
  },
  {
    title: "",
    fill: "#C7B8B7",
    icon: "/assets/face-with-look-of-triumf.svg",
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
