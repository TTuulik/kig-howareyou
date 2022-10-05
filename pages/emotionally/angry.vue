<script setup>
    import feelingsVue from './feelings.vue';
    
        definePageMeta({ layout: "emotionally" });
    </script>
    <template>
        <img src="/assets/css/Background.png" class="h-screen object-cover fixed -z-10" />
        <div style="display:flex; justify-content:center; align-items:center; min-height: 812px; height: 100%;">
            <div style="height:640px; width: 642px; background:#424F3DB2; display: flex; justify-content: center; align-items: center; flex-direction: column; text-align: center; padding: 0 10px 0 10px;">
                <h1 style="color:#fff; font-size:26px; padding-bottom: 24px;">How to deal with anger</h1>
                <div style="border-bottom: 9px dotted #00000040; width: 90px;"></div>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 28px;">Go for a walk</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Take deep breaths</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Listen to music</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Talk to someone</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Read a book</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Write about your feelings</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Ask yourself<br>if your anger is reasonable</p>
                <p style="color:#fff; text-align: center; font-size: 20px; padding-top: 19px;">Identify other emotions that your anger may be masking</p>
            </div>
            <nuxt-link to="/emotionally/feelings" style="position: absolute; left: 20px; bottom: 110px;">
                <img src="/assets/css/back.png" alt="back" class="w-8">
            </nuxt-link>
        </div>
    </template>
    