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
