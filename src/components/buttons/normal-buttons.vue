<template>
    <div>
        <button class="default">默认按钮</button>
        <button class="primary">主要按钮</button>
        <button class="text">文字按钮</button>
    
    </div>
</template>
<style scoped>
button {
    padding: 10px 20px;
    outline: 0;
    border-radius: 4px;
    cursor: pointer;
}

button.default {
    background: #fff;
    color: #000;
    border: 1px solid #bfcbd9;
}

button.default:hover {
    color: #20a0ff;
    border-color: #20a0ff;
}

button.default:active {
    border: 1px solid #bfcbd9;
    color: #000;
}

button.primary {
    background: #20a0ff;
    border: 1px solid #20a0ff;
    color: #fff;
}

button.primary:hover {
    background: #4db3ff;
    border-color: #4db3ff;
}

button.primary:active {
    background: #1d90e6;
    border: 1px solid #1d90e6;
}


button.text {
    background: #fff;
    border: 1px solid #fff;
    color: #20a0ff;
}

button.text:hover {
    color: #1d90e6;
}

button.text:active {
    color: #ccc;
}

</style>
<script>
export default {

}
</script>