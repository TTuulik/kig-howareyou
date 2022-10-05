<script setup>
    definePageMeta({ layout: "emotionally" });
</script>
<template>
    <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" />
    <div style="display:flex; justify-content:center; align-items:center; min-height: 812px; height: 100%;">
        <div style="height:640px; width: 642px; background:#424F3DB2; display: flex; justify-content: center; align-items: center; flex-direction: column; text-align: center; padding: 0 10px 0 10px;">
            <h1 style="color:#fff; font-size:26px; padding-bottom: 24px; text-align: center;">How to get over a<br>mental block</h1>
            <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 28px;">Go for a walk</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Listen to music</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Meditate</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Reduce stress</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Get an outside perspective</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Give yourself a break</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Calm your environment</p>
            <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Sleep</p>
        </div>
        <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 110px;">
            <img src="/assets/css/back.png" alt="back" class="w-8">
        </nuxt-link>
    </div>
</template>
