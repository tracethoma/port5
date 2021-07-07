<template>
    <div class="center">
        <div class="small_banner"><NuxtLink to="/">
            <div class="background-image-div"></div>
            <p class="">This is project {{ projectHomeBanner.title }}</p>
            
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1600 150" class="image">
                <defs>
                    <clipPath id="maskImage" clipPathUnits="objectBoundingBox" >
                        <!-- <rect x="0" y="0" width="1600" height="150"/> -->
                        <polygon fill="none" points="0,0 1,0 1, 1 0, 1 0, 1 "/>
                    </clipPath>
                </defs>
            </svg></NuxtLink>
        </div>
        <div class="spacer_projects"></div>
    </div>
</template>

<script>
    export default {
        props: {
            projectHomeBanner: {
            type: Object,
            default: null
            }
        }
        /* props: [ 'projectHomeBanner' ] */
    }

</script>

<style scoped>
    @import '~/assets/css/projects.css';
</style>