<script setup>
    const items = [
        {
            image:'assets/images/icon-target.svg',
            heading:'Focused on UX',
            des:'Use this area to list your app\'s key benefits. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. ',
        },
        {
            image:'assets/images/icon-rocket.svg',
            heading:'Convert Users',
            des:'Use this area to list your app\'s key benefits. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. ',
        },
        {
            image:'assets/images/icon-cogs.svg',
            heading:'Easy Customisations',
            des:'Use this area to list your app\'s key benefits. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. ',
        }
    ]

</script>

<template>
    <section class="benefits-section py-5">
        <div class="container py-lg-5">
            <h3 class="mb-5 text-center font-weight-bold">Market your mobile app effectively with Nova</h3>
            <div class="row">
                <template v-for="(item,index) in items"  :key="index">
                    <div class="item col-12 col-lg-4">
                        <div class="item-inner text-center p-3 p-lg-5">
                            <img class="mb-3 align-items-center" :src="item.image" alt="" />
                            <h5>{{item.heading}}</h5>
                            <div>{{item.des}}</div>
                        </div><!--//item-inner-->
                    </div><!--//item-->
                </template>
            </div><!--//row-->
            <div class="pt-3 text-center">
                <a class="btn btn-primary theme-btn theme-btn-ghost font-weight-bold" href="#">Learn More</a>
            </div>
        </div>

    </section><!--//benefits-section-->
</template>

<style scoped>

</style>