<template>
    <div>
        <SezioneLoghi/>
        <SezioneKey/>
    </div>
</template>

<script>
import SezioneLoghi from './SezioneLoghi.vue'
import SezioneKey from './SezioneKey.vue'
export default {
    name:'Main',
    components:{
        SezioneLoghi,
        SezioneKey,
    }
}
</script>

<style lang="scss" scoped>
h1{
    padding: 100px;
}
.wrapper {
  
}

</style>