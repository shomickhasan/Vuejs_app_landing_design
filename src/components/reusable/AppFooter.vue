<script setup>
    const footerElements = [
        {
            id:1,
            navheading:'About Nova',
            navItems:[
                'Our Story',
                'Pricing',
                'Contact',
                'Jobs',
            ],
        },
        {
            id: 2,
            navheading:'Resources',
            navItems:[
                'Home',
                'Profile',
                'About',
                'Contact',
            ],
        },

        {
            id: 3,
            navheading:'Legal',
            navItems:[
                'FAQs',
                'Blog',
                'Support',
                'Developer APIs',
            ],
        },
        {
            id: 4,
            navheading:'Stay Connected',
            navItems:[
                'fab fa-instagram fa-fw',
                'fab fa-twitter fa-fw',
                'fab fa-facebook-f fa-fw',
                'Developer APIs',
                'fab fa-youtube fa-fw',
            ],
        },
    ]

</script>
<template>
    <footer class="footer theme-bg-primary">
        <div class="container py-5 mb-3">
            <div class="row">
                 <div v-for="element in footerElements" :key="element.id" class="footer-col col-6 col-lg-3">
                     <h4 class="col-heading">{{element.navheading}}</h4>
                     <ul v-for="(navitem,index) in element.navItems" :key="index"  :class="(4 == element.id) ?['social-list','mb-0']:'list-unstyled'">
                         <li :class="(4==element.id) ? ['list-inline-item']:''"><a class="text-link" href="#">{{(4 != element.id ? navitem:'' )}} <span v-if="4==element.id"><i :class="navitem"></i></span></a></li>
                     </ul>
                 </div>
            </div><!--//footer-col-->
        </div><!--//row-->


        <div class="container">
            <hr>
        </div>
        <div class="download-area py-4">
            <div class="container text-center">
                <h3 class="mb-3">Get the app</h3>
                <div class="section-intro mb-4 single-col-max-width mx-auto">Download our apps now. lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis. </div>
                <ul class="app-stores list-unstyled list-inline mx-auto  d-inline-block">
                    <li class="list-inline-item me-3"><a href="#"><img class="ios" src="assets/images/appstore-apple.svg" alt="app-store"></a></li>
                    <li class="list-inline-item"><a href="#"><img class="android" src="assets/images/appstore-android.svg" alt="google play"></a></li>
                </ul>
            </div><!--//container-->
        </div><!--//download-area-->
        <div class="footer-bottom text-center pb-5">
            <!--/* This template is free as long as you keep the footer attribution link. If you'd like to use the template without the attribution link, you can buy the commercial license via our website: themes.3rdwavemedia.com Thank you for your support. :) */-->
            <small class="copyright">Designed with <span class="sr-only">love</span><i class="fas fa-heart" style="color: #fb866a;"></i> by <a href="http://themes.3rdwavemedia.com" target="_blank">Xiaoying Riley</a> for developers</small>
        </div>
    </footer>
</template>

<style scoped>

</style>