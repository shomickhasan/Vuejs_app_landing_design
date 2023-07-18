<script setup>
//import backgroundImg from 'assets/images/hero-figure.png'
const  backgroundimage= `background:url('assets/images/hero-figure.png') no-repeat right top;background-size:480px auto;min-height:600px}`
const heroContent ={
    headline:`The best way to promote your app and convert users.`,
    tagLine:`High converting Bootstrap landing page template made for app developers. Built with Bootstrap 5 and Sass. Get started now!`,
}
const appStoreImages = [
    `assets/images/appstore-apple.svg`,
    `assets/images/appstore-android.svg`,
]




</script>
<template >
    <section class="hero-section">
        <div class="container">
            <div class="row figure-holder" :style="backgroundimage">
                <div class="col-12 col-md-6 pt-3 pt-md-4">
                    <h2 class="site-headline font-weight-bold mt-lg-5 pt-lg-5">{{heroContent.headline}}</h2>
                    <div class="site-tagline mb-3">{{heroContent.tagLine}}</div>
                    <div class="cta-btns">
                        <div class="mb-4"><a class="btn btn-primary font-weight-bold theme-btn" href="https://themes.3rdwavemedia.com/bootstrap-templates/startup/nova-bootstrap-landing-page-template-for-mobile-apps/">Try Nova for FREE</a></div>
                        <ul class="app-stores list-unstyled list-inline mx-auto mx-md-0 d-inline-block">
                            <li v-for="appStoreImage in appStoreImages" class="list-inline-item me-3"><a href="#"><img class="ios" :src="appStoreImage" alt="app-store"></a></li>
                        </ul>
                    </div>
                    <img :src="backgroundimage" alt="">
                </div>
            </div><!--//row-->
        </div>
    </section><!--//hero-section-->
</template>
<style scope>
  
</style>
