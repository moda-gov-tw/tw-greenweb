<script setup>
import FrontLayout from '@/Layouts/FrontLayout.vue';
import { Head } from '@inertiajs/vue3';

const props = defineProps({
    title: String,
})

</script>

<template>

    <Head :title="props.title" />
    <FrontLayout>

        <div class="container text-center">
            <div class="text-center wow fadeInUp display_flex">
                <a href="#C" name="C" title="中間區域" accesskey="C" style="padding: 25px 0; color: #fff;">:::</a>
                <h1 class="carbon_gold ctca-font carbon_title" style="padding-top: 25px; font-size: 1.8em;">網頁碳排計算器</h1>
            </div>
        </div>

        <div class="container" style="padding-top: 2rem; text-align: center;">
            <p class="ctca-font" style="font-size: 1.3em; font-weight: 700; color: white;">
                你知道，網頁也會產生碳排放量嗎?
            </p>
        </div>

        <div class="container" style="padding-top: 1.1rem; text-align: center;">
            <p class="ctca-font" style="font-size: 1.1em; font-weight: 700; color: white; text-indent: 2em;">
                全球的網際網路消耗了大量電力，大約每年1021太瓦時(TWh)，這是全台灣整年度用電量2794.5億度的3650倍之多。從資料中心到網路傳輸過程，再到我們手中的數十億個連線裝置，都一直不斷地消耗電力，而這其中所產生的碳排放量幾乎等於全球航空業所產生的碳排放！
            </p>
        </div>

        <div class="container" style="text-align: center;">
            <p class="ctca-font" style="font-size: 1.1em; font-weight: 700; color: white; text-indent: 2em;">
                本站所開發的「網頁碳排計算器」，可以協助大家估算自己設計或瀏覽的網頁產生了多少的碳排放量，估算結果雖然並非是一個非常精準的數據，但希望可以透過這樣的量化工具，具體呈現網頁所產生的碳排量，讓所有人可以建立起數位行為之綠色意識，並用更永續的方式來設計與使用網際網路！
            </p>
        </div>

        <div class="container" style="text-align: center;">
            <p class="ctca-font" style="font-size: 1.1em; font-weight: 700; color: white; text-indent: 2em;">
                （想了解更多請參考本案產出之<a href="/gain/58/8" title="導向網路永續設計指引">網路永續設計指引</a>）
            </p>
        </div>

    </FrontLayout>
</template>

<style scoped>
.img-fluid {
    width: 70%;
}
</style>
