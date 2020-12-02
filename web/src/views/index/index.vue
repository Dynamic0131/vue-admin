<template>
    <div>
        <Cars />
        <Map />
        <!-- 会员 -->
        <div id="children-view">
            <router-view />
        </div>
    </div>
</template>
<script>
import Map from "../amap"
import Cars from "../cars"
export default {
    name: "Index",
    components: {
        Map,
        Cars
    },
    data(){
        return {}
    }
}
</script>
<style lang="scss">
#children-view {
    position: fixed;
    top: 0;
    bottom: 0;
    right: 0;
    z-index: 101;
    width: 410px;
    background-color: #34393f;
}
</style>