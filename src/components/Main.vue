<template>
    <main>

        <!-- sezione 1 -->
        <SezioneLoghi/>
        <!-- /sezione 1 -->

        <!-- sezione 2 -->
        <SezioneKey/>
        <!-- /sezione 2 -->

        <!-- sezione 3 -->
        <SezioneTools/>
        <!-- /sezione 3 -->

        <!-- sezione 4 -->
        <SezioneShop/>
        <!-- /sezione 4 -->

        <!-- sezione 5 -->
        <SezioneInfoEmail/>
        <!-- /sezione 5 -->

    </main>
</template>

<script>
// import componenti
import SezioneLoghi from './SezioneLoghi.vue'
import SezioneKey from './SezioneKey.vue'
import SezioneTools from './SezioneTools.vue'
import SezioneShop from './SezioneShop.vue'
import SezioneInfoEmail from './SezioneInfoEmail.vue'

export default {
    name:'Main',
    components:{
        SezioneLoghi,
        SezioneKey,
        SezioneTools,
        SezioneShop,
        SezioneInfoEmail

    }
}
</script>

<style lang="scss" scoped>

</style>