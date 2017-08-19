<template>
    <div>
    
        <button class="default disabled"  disabled="disabled">默认按钮</button>
        <button class="primary disabled"  disabled="disabled">主要按钮</button>
        <button class="text disabled"  disabled="disabled">文字按钮</button>
    </div>
</template>
<style scoped>
button {
    padding: 10px 20px;
    outline: 0;
    border-radius: 4px;
    cursor: pointer;
}
button.disabled {
    cursor: not-allowed;
    color: #d1dbe5;
}
button.text.disabled {
    color: #d1dbe5;
    border:0;
    background: #fff;
}
button.primary.disabled {
    background-color: #eef1f6;
    border:1px solid #d1dbe5;
}
button.default.disabled {
    background: #fff;
    border:1px solid #d1dbe5;
    color: #d1dbe5;
}
</style>
<script>
export default {

}
</script>