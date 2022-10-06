<script setup>
    import musicVue from './music.vue';
    definePageMeta({ layout: "emotionally" });
</script>
<template>
    <div>
        <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" style="width:100%;"/>
        <div style="display:flex; justify-content:center; align-items:center; height: 100vh;">
            <div style="height:640px; width: 100%; background:#424F3DB2; display: flex; justify-content: flex-start; align-items: center; flex-direction: column; text-align: center; padding: 20px 10px 0 10px;">
                <h1 style="color:#fff; font-size:26px; padding-bottom: 24px; text-align: center;">What to do when you're confused</h1>
                <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 24px;">Try not to panic and relax</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Take a deep breath</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Talk or write about your thoughts</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Engage in compassionate self talk</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Focus on present</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Distract yourself temporarily</p>
                <nuxt-link to="/emotionally/exercise"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Try musical relaxation &#8594</p></nuxt-link>
                <nuxt-link to="/emotionally/exercise"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">5-4-3-2-1 Grounding Exercise &#8594</p></nuxt-link>
            </div>
            <nuxt-link to="/emotionally/feelings">
                <div style="position: absolute; left: 20px; bottom: 20px;">
                    <img src="/assets/css/back.png" alt="back" class="w-8">
                </div>
            </nuxt-link>
        </div>
    </div>
</template>
