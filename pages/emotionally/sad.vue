<script setup>
        definePageMeta({ layout: "emotionally" });
    </script>
    <template>
        <div>
            <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" style="width:100%;"/>
            <div style="display:flex; justify-content:center; align-items:center; min-height: 812px; height: 100%;">
                <div style="height:640px; width: 642px; background:#424F3DB2; display: flex; justify-content: flex-start; align-items: center; flex-direction: column; text-align: center; padding: 20px 10px 0 10px;">
                    <h1 style="color:#fff; font-size:26px; padding-bottom: 24px;">Things to do when<br>you're sad</h1>
                    <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 25px;">Cry</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Dance to your favorite song</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Hang out with your friends</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Set goals and create change</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Meet new people</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Do something you've always<br>wanted to do</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Explore the magical outdoors</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Write about your feelings</p>
                    <nuxt-link to="/emotionally/music"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Listen to beautiful music &#8594</p></nuxt-link>
                    <nuxt-link to="/emotionally/meditate"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Meditate &#8594</p></nuxt-link>
                </div>
                <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 20px;">
                    <img src="/assets/css/back.png" alt="back" class="w-8">
                </nuxt-link>
            </div>
        </div>
    </template>
    