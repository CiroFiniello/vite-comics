<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
    data() {
        return 
            {
        }
    },
        components:{
            AppHeader,
            AppMain,
            AppFooter
        
    }
}
</script>

<template>

<AppHeader />
<AppMain />
<AppFooter />

</template>

<style >
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
</style>