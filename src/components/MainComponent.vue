<template>
    <div class="card"  @click="flipCard">
        <div :class="card.flip ? 'back' : 'front'"></div>
    </div>
</template>
<script>
export default {
    name: 'OpenComponent',

    data() {
        return {
            card: {
                flip:false
            }
        }
    },
    methods: {
        // 카드 뒤집는 메소드
        flipCard(){
            this.card.flip = !this.card.flip
        }
    }
}
</script>

<style lang="/public/css/common.css">

</style>