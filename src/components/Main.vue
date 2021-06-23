<template>
    <main>
        
        <SezioneLoghi/>
        <SezioneKey/>
        <SezioneTools/>
        <SezioneShop/>
        <SezioneInfoEmail/>
        
    </main>
</template>

<script>
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