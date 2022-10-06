<script setup>
definePageMeta({ layout: "default" });

const start = [
  {
    goto: "down",
    title: "",
    fill: "lightblue",
    largeicon: "/assets/confused-face.svg",
  },
  {
    goto: "up",
    title: "",
    fill: "yellow",
    largeicon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
];

const up = [
  {
    goto: "up2",
    title: "",
    fill: "#FFCC80",
    icon: "/assets/smiling-face-with-smiling-eyes.svg",
  },
  {
    goto: "up2",
    title: "",
    fill: "#FDBA74",
    icon: "/assets/smiling-face-with-heart-shaped-eyes.svg",
  },
  {
    goto: "up2",
    title: "",
    fill: "#FDE68A",
    icon: "/assets/smiling-face-with-halo.svg",
  },
  {
    goto: "up2",
    title: "",
    fill: "#FECDD3",
    icon: "/assets/face-with-open-mouth.svg",
  },
  {
    goto: "up2",
    title: "",
    fill: "#FFBB89",
    icon: "/assets/face-with-stuck-out-tongue-and-tightly-closed-eyes.svg",
  },
  {
    goto: "up2",
    title: "",
    fill: "#FED7AA",
    icon: "/assets/face-savouring-delicious-food.svg",
  },
  {
    goto: "up2",
    title: "",
    fill: "#FECACA",
    icon: "/assets/grinning-face.svg",
  },
];

const up2 = [
  {
    goto: "start",
    title: "Jaga sõpradega!",
    fill: "#FEF08A",
    icon: "",
  },
  {
    goto: "start",
    title: "Mul on su üle hea meel!",
    fill: "#FDBA74",
    icon: "",
  },
  {
    goto: "start",
    title: "Äge!",
    fill: "#FDE047",
    icon: "",
  },
  {
    goto: "start",
    title: "Tähista!",
    fill: "#FECDD3",
    icon: "",
  },
];

const down = [
  {
    goto: "down3",
    title: "",
    fill: "purple",
    icon: "/assets/angry-face.svg",
  },
  {
    goto: "down3",
    title: "",
    fill: "#C7B8B7",
    icon: "/assets/confounded-face.svg",
  },
  {
    goto: "down3",
    title: "",
    fill: "skyblue",
    icon: "/assets/confused-face.svg",
  },
  {
    goto: "down3",
    title: "",
    fill: "purple",
    icon: "/assets/disappointed-but-relieved-face.svg",
  },
  {
    goto: "down3",
    title: "",
    fill: "#C7B8B7",
    icon: "/assets/expressionless-face.svg",
  },
  {
    goto: "down3",
    title: "",
    fill: "purple",
    icon: "/assets/loudly-crying-face.svg",
  },
  {
    goto: "down3",
    title: "",
    fill: "#9FA1A1",
    icon: "/assets/tired-face.svg",
  },
  {
    goto: "down3",
    title: "",
    fill: "skyblue",
    icon: "/assets/face-with-look-of-triumph.svg",
  },
];

const down2 = [
  {
    goto: "down4",
    title: "",
    fill: "#DFF996",
    largeicon: "/assets/leaf-outline.svg",
  },
  {
    goto: "down4",
    title: "",
    fill: "#FEF08A",
    largeicon: "/assets/artist-palette.svg",
  },
  {
    goto: "down4",
    title: "",
    fill: "#BBF7D0",
    largeicon: "/assets/brain.svg",
  },
  {
    goto: "down4",
    title: "",
    fill: "#F5E3A0",
    largeicon: "/assets/body-outline.svg",
  },
];

const down3 = [
  {
    goto: "down2",
    title: "MURE",
    fill: "skyblue",
  },
  {
    goto: "down2",
    title: "SEGADUS",
    fill: "#E5E7EB",
  },
  {
    goto: "down2",
    title: "ALANDUS",
    fill: "#CBD5E1",
  },
  {
    goto: "down2",
    title: "KAHETSUS",
    fill: "#E5E7EB",
  },
];

const down4 = [
  {
    goto: "start",
    title: "Räägi oma taimedega.",
    fill: "#DFF996",
  },
  {
    goto: "start",
    title: "Mine õue!",
    fill: "#FEF08A",
  },
  {
    goto: "start",
    title: "Vaata 3 min aknast välja",
    fill: "#BBF7D0",
  },
  {
    goto: "start",
    title: "Mine jaluta 30. min",
    fill: "#F5E3A0",
  },
];

const page = $ref("start");
const onSelect = (selection) => {
  page = selection.goto || "start";
};
</script>

<template>
  <div class="">
    <div>
      <div>{{ page }}</div>
      <!-- <button class="startbtn"><img src="/assets/back-btn.svg" /></button> -->
      <TestWheel v-if="page == 'start'">
        <TestSlices
          :options="start"
          :inner="2"
          :outer="150"
          :corner="5"
          :padding="2"
          @select="onSelect"
        />
      </TestWheel>
      <TestWheel v-if="page == 'up'">
        <TestSlices
          :options="up"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
          @select="onSelect"
        />
      </TestWheel>
      <TestWheel v-if="page == 'up2'">
        <TestSlices
          :options="up2"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
          @select="onSelect"
        />
      </TestWheel>
      <TestWheel v-if="page == 'down'">
        <TestSlices
          :options="down"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
          @select="onSelect"
        />
      </TestWheel>
      <TestWheel v-if="page == 'down2'">
        <TestSlices
          :options="down2"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
          @select="onSelect"
        />
      </TestWheel>

      <TestWheel v-if="page == 'down3'">
        <TestSlices
          :options="down3"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
          @select="onSelect"
        />
      </TestWheel>

      <TestWheel v-if="page == 'down4'">
        <TestSlices
          :options="down4"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
          @select="onSelect"
        />
      </TestWheel>
    </div>
  </div>
</template>
