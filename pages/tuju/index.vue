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
    title: "",
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
    title: "Jaga sõpradega!",
    fill: "#FEF08A",
    icon: "",
  },
  {
    title: "Mul on su üle hea meel!",
    fill: "#FDBA74",
    icon: "",
  },
  {
    title: "Äge!",
    fill: "#FDE047",
    icon: "",
  },
  {
    title: "Tähista!",
    fill: "#FECDD3",
    icon: "",
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
    fill: "#C7B8B7",
    icon: "/assets/confounded-face.svg",
  },
  {
    title: "",
    fill: "skyblue",
    icon: "/assets/confused-face.svg",
  },
  {
    title: "",
    fill: "purple",
    icon: "/assets/disappointed-but-relieved-face.svg",
  },
  {
    title: "",
    fill: "#C7B8B7",
    icon: "/assets/expressionless-face.svg",
  },
  {
    title: "",
    fill: "purple",
    icon: "/assets/loudly-crying-face.svg",
  },
  {
    title: "",
    fill: "#9FA1A1",
    icon: "/assets/tired-face.svg",
  },
  {
    title: "",
    fill: "skyblue",
    icon: "/assets/face-with-look-of-triumph.svg",
  },
];

const down2 = [
  {
    title: "",
    fill: "#DFF996",
    icon: "/assets/leaf-outline.svg",
  },
  {
    title: "",
    fill: "#FEF08A",
    icon: "/assets/artist-palette.svg",
  },
  {
    title: "",
    fill: "#BBF7D0",
    icon: "/assets/brain.svg",
  },
  {
    title: "",
    fill: "#F5E3A0",
    icon: "/assets/body-outline.svg",
  },

  
];

const down3 = [
{
    title: "MURE",
    fill: "skyblue",
    
  },
  {
    title: "SEGADUS",
    fill: "#E5E7EB",
    
  },
  {
    title: "ALANDUS",
    fill: "#CBD5E1",
    
  },
  {
    title: "KAHETSUS",
    fill: "#E5E7EB",
  
  },

];

const down4 = [
  {
    title: "Räägi oma taimedega.",
    fill: "#DFF996",
  },
  {
    title: "Mine õue!",
    fill: "#FEF08A",
  },
  {
    title: "Vaata 3 min aknast välja",
    fill: "#BBF7D0",
  },
  {
    title: "Mine jaluta 30. min",
    fill: "#F5E3A0",
  },

  
];

</script>

<template>
  <div class="">
    <div>
      <div>Start</div>
            <button><img src="/assets/back-btn.svg"></button>
      <TestWheel>
        <TestSlices
          :options="start"
          :inner="2"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
      <div>Up</div>
            <button><img src="/assets/back-btn.svg"></button>
      <TestWheel>
        <TestSlices
          :options="up"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
      <div>Up2</div>
            <button><img src="/assets/back-btn.svg"></button>
      <TestWheel>
        <TestSlices
          :options="up2"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
      <div>Down</div>
            <button><img src="/assets/back-btn.svg"></button>
      <TestWheel>
        <TestSlices
          :options="down"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>
      <div>Abiks</div>
            <button><img src="/assets/back-btn.svg"></button>
      <TestWheel>
        <TestSlices
          :options="down2"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>

      <div>Down3</div>
            <button><img src="/assets/back-btn.svg"></button>
      <TestWheel>
        <TestSlices
          :options="down3"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>

      <div>Paus</div>
            <button><img src="/assets/back-btn.svg"></button>
      <TestWheel>
        <TestSlices
          :options="down4"
          :inner="4"
          :outer="150"
          :corner="5"
          :padding="2"
        />
      </TestWheel>

    </div>
  </div>
</template>
