<script setup>
    definePageMeta({ layout: "emotionally" });
</script>
<template>
    <div>
        <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" />
        <div style="display:flex; justify-content:center; align-items:center; min-height: 812px; height: 100%;">
            <div style="height:640px; width: 642px; background:#424F3DB2; display: flex; justify-content: flex-start; align-items: center; flex-direction: column; text-align: center; padding: 20px 10px 0 10px;">
                <h1 style="color:#fff; font-size:26px; padding-bottom: 24px; text-align: center;">5-4-3-2-1<br>Grounding Exercise</h1>
                <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 24px;">When you're dealing with<br>confusion, this is a great method<br>for clearing your head and<br>improving focus.<br><br>Engage all five senses and<br>mindfully notice five things you<br>can see, four things you can<br>touch, three things you can hear,<br>two things you can smell, and<br>one thing you can taste. Go in<br>any order that makes sense for<br>you and your current situation<br>- no pressure!</p>
            </div>
            <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 20px;">
                <img src="/assets/css/back.png" alt="back" class="w-8">
            </nuxt-link>
        </div>
    </div>
</template>
