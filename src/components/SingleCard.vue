<script>
export default {
    data() {
        return 
            {

        }
    },
    props: {
        singleCard:{
            type: Object,
            required: true
        }
    }
}
</script>

<template>
<article>

    <img :src="singleCard.thumb" :alt="singleCard.series">
                    <h4>
                        {{ singleCard.series }}
                    </h4>
</article>

</template>

<style lang="scss" scoped>
        article{
            width: calc(100% / 6);
            img{
                width: 100%;
                padding: 1rem;
            }
        }
</style>