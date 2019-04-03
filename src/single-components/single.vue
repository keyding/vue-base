<template>
    <div class="single_container">
        <div class="tip">{{ message }}</div>
    </div>
</template>

<script>
export default {
    name: 'Single',
    data () {
        return {
            message: '酷云互动是新一代电视媒体大数据平台的开创者和领导者'
        }
    }
}
</script>

<style scoped>
.single_container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 400px;
}

.single_container .tip {
    display: flex;
    align-items: center;
    width: 400px;
    height: 30px;
    font-size: 14px;
    padding: 0 20px;
    border-radius: 4px;
    border: 1px solid #ccc;
}
</style>


