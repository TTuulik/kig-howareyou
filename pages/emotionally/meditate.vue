<script setup>
        definePageMeta({ layout: "emotionally" });
    </script>
    <template>
        <div>
            <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" />
            <div style="display:flex; justify-content:center; align-items:center; min-height: 812px; height: 100%;">
                <div style="height:640px; width: 642px; background:#424F3DB2; display: flex; justify-content: flex-start; align-items: center; flex-direction: column; text-align: center; padding: 20px 10px 0 10px;">
                    <h1 style="color:#fff; font-size:26px; padding-bottom: 24px;">Meditate</h1>
                    <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 24px;">Set a time limit</p>
                    <p style="color:#fff; text-align: center; font-size: 13px;">If you're just beginning, it can help to choose a<br>short time, such as five or 10 minutes.</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Find a place where to sit that feels calm and quiet to you</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Feel your breath</p>
                    <p style="color:#fff; text-align: center; font-size: 13px;">Follow the sensation of your breath<br>as it goes in and as it goes out.</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Be kind to your wandering mind</p>
                    <p style="color:#fff; text-align: center; font-size: 13px;">Don't judge yourself or obsess over the content<br>of the thoughts you find yourself lost in.</p>
                    <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Close with kindness</p>
                    <p style="color:#fff; text-align: center; font-size: 13px;">When you're ready, gently lift your gaze. Take a moment and notice any sounds in the environment. Notice how your body feels right now. Notice your thoughts and emotions.</p>
                    <nuxt-link to="/emotionally/music"><p style="color:#fff; text-align: center; font-size: 20px; padding-top: 14px;">Music &#8594</p></nuxt-link>
                </div>
                <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 20px;">
                    <img src="/assets/css/back.png" alt="back" class="w-8">
                </nuxt-link>
            </div>
        </div>
    </template>
