<script setup>
    const items = [
        'fab fa-twitter fa-fw',
        'fab fa-facebook-f fa-fw',
        'fab fa-instagram fa-fw',
    ]
    const bannerInfo = {
        heading: 'Love this template? Need more page designs?',
        link: 'https://themes.3rdwavemedia.com/bootstrap-templates/mobile/bootstrap-template-for-mobile-apps-nova-pro/',
        vertionName: 'Nova Pro',
        buttonText:'Check out',
    }
    const brand ={
        icon: 'assets/images/logo-icon.svg',
        brandText1: 'NOVA',
        text2:'Pro'
    }
</script>
<template>
    <div class="demo-banner py-3 text-white text-center fw-bold theme-bg-secondary text-white">{{bannerInfo.heading}} <a class="btn font-weight-bold ms-2 theme-btn-on-bg mt-2 mt-md-0" :href="bannerInfo.link" target="_blank"><i class="fas fa-external-link-alt me-2"></i>{{bannerInfo.buttonText}} <span class="text-uppercase">{{bannerInfo.vertionName}}</span></a>
    </div>
    <header class="header">
        <div class="branding">
            <div class="container position-relative">
                <nav class="navbar navbar-expand-lg" >
                    <h1 class="site-logo"><a class="navbar-brand" href="/"><img class="logo-icon" :src="brand.icon" alt="logo"> <span class="logo-text">{{brand.brandText1}} <span class="alt rounded">{{brand.text2}}</span></span></a></h1>
                    <ul class="social-list list-inline mb-0 position-absolute">
                        <li v-for="(item,index) in items" class="list-inline-item" :class="item" :key="index"><a class="text-dark" href="#"><i class=""></i></a></li>
                    </ul><!--//social-list-->
                </nav>
            </div><!--//container-->
        </div><!--//branding-->
    </header><!--//header-->
</template>
<style scoped>

</style>