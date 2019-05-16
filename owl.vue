<template>
    <div class="container-fluid">
        <no-ssr>
            <Owl :options="options">
                <div class="item">
                    <img src="http://fpoimg.com/600x250/For%20Place%20Only%20Image" alt="">            
                </div>
                <div class="item">
                    <img src="http://fpoimg.com/600x250/For%20Place%20Only%20Image" alt="">            
                </div>
            </Owl>
        </no-ssr>
    </div>
</template>

<script>
    import Owl from '~/components/OwlCarouselBox';

    export default {
        head: {
            bodyAttrs: {
                class: 'subpage'
            }
        },
        components: {
            Owl: Owl
        },
        data() {
            return {
                options: {
                    items: 1,
                    autoplay: false,
                    loop: true,
                    items: 1,
                    margin: 0,
                    nav:true,
                    dots:false
                }
            }
        },
    }

</script>
