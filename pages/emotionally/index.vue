<script setup>
// setTimeout(async () => await navigateTo("/emotionally/feelings"), 1000);
definePageMeta({ layout: "emotionally" });
</script>
<template>
  <div>
    <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" style="width:100%;"/>
    <div style="display: flex; justify-content: center; align-items: center; width: 100%; height: 100vh;">
      <nuxt-link to="/emotionally/feelings" style="height: 185px; width: 100%; background: #424f3db2; display: flex; justify-content: center; align-items: center; flex-direction: column; box-shadow: inset 0px -4px 4px rgba(0, 0, 0, 0.25), inset 0px 4px 4px rgba(0, 0, 0, 0.25);">
        <img src="/assets/css/Logo.png" alt="Emotionally logo" class="w-64" />
        <p style="color: #fff; text-align: center; font-size: 16px">
          To guide your body and heal your mind
        </p>
      </nuxt-link>
    </div>
  </div>
</template>
