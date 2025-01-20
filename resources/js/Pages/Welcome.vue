<script setup>
import FrontLayout from '@/Layouts/FrontLayout.vue';
import { Head, router } from '@inertiajs/vue3';
import LinkError from '@/Components/LinkError.vue';
import { ref, onUnmounted } from 'vue';
import axios from 'axios';
import SwiperCarouselVue from "@/Components/SwiperCarousel.vue";

const timer = ref()

const url = ref('https://')

const errors = ref('')

const button_state = ref(false)

const props = defineProps({
    title: String,
})

onUnmounted(() => {
    clearTimeout(timer.value)
    timer.value = ''
})

</script>

<template>

    <Head :title="props.title" />
    <FrontLayout>
        <!-- <div class="container-xxl p-0 mb-3">
            <SwiperCarouselVue />
        </div> -->

        <div class="container-xxl py-5">
            <div class="container">
                <div class="row g-5">
                    <div class="col-lg-5 pt-4">
                        <a href="#C" name="C" accesskey="C" id="ace_m" target="_self" title="中間區域"
                            style="color: #fff;">:::</a>
                        <a href="/" class="ctca-font ctca-font-size-title" title="到首頁">首頁</a>
                    </div>
                </div>
            </div>
        </div>

        <div class="container" style="padding-top: 2rem; text-align: center;">
            <p class="ctca-font" style="font-size: 1.3em; font-weight: 700; color: white;">
                你知道，網頁也會產生碳排放量嗎?
            </p>
        </div>

        <div class="container" style="padding-top: 1.1rem; text-align: center;">
            <p class="ctca-font" style="font-size: 1.1em; font-weight: 700; color: white; text-indent: 2em;">
                網際網路已是現代生活不可或缺的一部分，但其隱藏的碳排放問題卻常被忽視。為了更直觀地了解網頁瀏覽或設計對環境的影響。本網站開發了「網頁碳排計算器」來計算網頁運行的碳排放，藉此提升社會對於數位行為及環境影響的認識。
            </p>
        </div>

        <div class="container" style="text-align: center;">
            <p class="ctca-font" style="font-size: 1.1em; font-weight: 700; color: white; text-indent: 2em;">
                同時我們提供「網際網路永續設計指引」，透過具體的網頁設計原則與建議，協助網站設計者以簡潔與高效的方式來降低碳排放，推動技術創新與永續理念的結合，實現環境永續與數位轉型的雙贏。
            </p>
        </div>

        <div class="container" style="text-align: center;">
            <p class="ctca-font" style="font-size: 1.1em; font-weight: 700; color: white; text-indent: 2em;">
                （想了解更多請參考本網站產出之<a href="/gain/58/8" title="導向網路永續設計指引">網際網路永續設計指引</a>）
            </p>
        </div>

    </FrontLayout>
</template>

<style scoped>
.img-fluid {
    width: 70%;
}
</style>
