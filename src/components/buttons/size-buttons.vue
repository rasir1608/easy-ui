<template>
    <div>
        <button class="primary large">大型按钮</button>
        <button class="primary">正常按钮</button>
        <button class="primary small">小型按钮</button>
        <button class="primary mini">超小型按钮</button>
    </div>
</template>
<style scoped>
button {
    padding: 10px 20px;
    outline: 0;
    border-radius: 4px;
    cursor: pointer;
}

/* 大型按钮 */
button.large{
    padding:13px 20px;
    font-size: 16px;
}

/* 小型按钮 */
button.small{
    padding: 5px 10px;
}

/* 超小型按钮 */
button.mini{
    padding: 2px 2px;
     font-size: 12px;
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

</style>
<script>
export default {

}
</script>