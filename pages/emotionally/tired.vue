<script setup>
    definePageMeta({ layout: "emotionally" });
</script>
<template>
    <div>
        <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" style="width:100%;"/>        <div style="display:flex; justify-content:center; align-items:center; height: 100vh;">
            <div style="display: flex; justify-content: flex-start; align-items: center; flex-direction: column; height:640px; width: 100%; background:#424F3DB2; text-align: center; padding: 20px 10px 0 10px;">
                <h1 style="color:#fff; font-size:26px; padding-bottom: 24px;">Tips for when you're tired</h1>
                <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 24px;">Reduce stress to boost energy</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Cut out caffeine</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Rule out health problems</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Drink more water for better energy</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Eat several small meals<br>instead of large, heavy ones</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Make an effort to move more </p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Prioritize your sleep</p>
            </div>
            <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 20px;">
                <img src="/assets/css/back.png" alt="back" class="w-8">
            </nuxt-link>
        </div>
    </div>
</template>
