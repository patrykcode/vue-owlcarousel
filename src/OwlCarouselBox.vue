<template>
    <div>
        <div v-bind:id="owlID.id" v-bind:class="owlID.class">
            <slot></slot>
        </div>
    </div>
</template>
<script>

    import 'owl.carousel/dist/assets/owl.carousel.css';
    import 'owl.carousel/dist/assets/owl.theme.default.css';
    import 'owl.carousel';

    export default {
        name: 'OwlCarouselBox',
        data: function () {
            return {}
        },
        props: {
            options: {
                default() {
                    return {}
                }
            },
            owlID: {
                default() {
                    return {
                        id: 'owl_' + (new Date().getTime()),
                        class: 'owl-carousel owl-theme'
                    };
                }
            },

        },
        mounted() {
            $('#' + this.owlID.id).owlCarousel(this.options);
        }
    }
</script>

