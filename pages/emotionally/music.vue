<script setup>
    definePageMeta({ layout: "emotionally" });
</script>
<template>
    <div>
        <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" style="width:100%;"/>
        <div style="display:flex; justify-content:center; align-items:center; min-height: 812px; height: 100%;">
            <div style="height:640px; width: 642px; background:#424F3DB2; display: flex; justify-content: flex-start; align-items: center; flex-direction: column; text-align: center; padding: 20px 10px 0 10px;">
                <h1 style="color:#fff; font-size:26px; padding-bottom: 24px; text-align: center;">Music</h1>
                <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
                <a href="https://open.spotify.com/artist/3jiEUUVkagxAsSpQaJWi3d"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 24px;">Meditate and chill &#8594</p></a>
                <a href="https://open.spotify.com/album/5nncRcV2N2W8KdoeLzTjJq"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Brain stimulating &#8594</p></a>
                <a href="https://open.spotify.com/album/2Kq1yt9vgjnYAA4t9hGRDw"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Hypnosis and relaxation &#8594</p></a>
                <a href="https://open.spotify.com/artist/7kMy7EALl5gVfGs1TgwuVI"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Plant wave &#8594</p></a>
            </div>
            <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 20px;">
                <img src="/assets/css/back.png" alt="back" class="w-8">
            </nuxt-link>
        </div>
    </div>
</template>
