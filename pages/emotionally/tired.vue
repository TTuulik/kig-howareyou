<script setup>
import feelingsVue from './feelings.vue';

    definePageMeta({ layout: "emotionally" });
</script>
<template>
    <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" />
    <div style="display:flex; justify-content:center; align-items:center; min-height: 812px; height: 100%;">
        <div style="height:640px; width: 642px; background:#424F3DB2; display: flex; justify-content: center; align-items: center; flex-direction: column; text-align: center; padding: 0 10px 0 10px;">
            <h1 style="color:#fff; font-size:26px; padding-bottom: 24px;">Tips for when you're tired</h1>
            <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 24px;">Reduce stress to boost energy</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Cut out caffeine</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Rule out health problems</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Drink more water for better energy</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Eat several small meals<br>instead of large, heavy ones</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Make an effort to move more </p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Prioritize your sleep</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Drink more water</p>
        </div>
        <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 20px;">
            <img src="/assets/css/back.png" alt="back" class="w-8">
        </nuxt-link>
    </div>
</template>
