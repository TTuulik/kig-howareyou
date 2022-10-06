<script setup>
    import feelingsVue from './feelings.vue';
    import musicVue from './music.vue';
    
    definePageMeta({ layout: "emotionally" });
</script>
<template>
    <div>
        <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" style="width:100%;"/>        <div style="display:flex; justify-content:center; align-items:center; height: 100vh;">
            <div style="height:640px; width: 100%; background:#424F3DB2; display: flex; justify-content: flex-start; align-items: center; flex-direction: column; text-align: center; padding: 20px 10px 0 10px;">
                <h1 style="color:#fff; font-size:26px; padding-bottom: 24px; text-align: center;">How to get over a<br>mental block</h1>
                <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 24px;">Go for a walk</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Reduce stress</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Get an outside perspective</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Give yourself a break</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Calm your environment</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Sleep</p>
                <nuxt-link to="/emotionally/music"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Listen to music &#8594</p></nuxt-link> 
                <nuxt-link to="/emotionally/exercise"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">5-4-3-2-1 Grounding Exercise &#8594</p></nuxt-link>
                <nuxt-link to="/emotionally/meditate"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Meditate &#8594</p></nuxt-link>
            </div>
            <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 20px;">
                <img src="/assets/css/back.png" alt="back" class="w-8">
            </nuxt-link>
        </div>
    </div>
</template>
