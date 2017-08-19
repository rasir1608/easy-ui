<template>
    <div>
        <button class="text success">成功按钮</button>
        <button class="text warning">警告按钮</button>
        <button class="text danger">危险按钮</button>
        <button class="text info">信息按钮</button>
    </div>
</template>
<style scoped>
button {
    padding: 10px 20px;
    outline: 0;
    border-radius: 4px;
    cursor: pointer;
}

button.success.text,
button.warning.text,
button.danger.text,
button.info.text {
    background: #fff;
    border: 1px solid #bfcbd9;
    color: #1f2d3d;
}



/* 成功按钮 */

button.success:hover {
    border-color: #42d885;
    color: #42d885;
}

button.success:active {
    border: 1px solid #11b95c;
    color: #11b95c;
}





/* 警告按钮 */

button.warning:hover {
    border-color: #f9c855;
    color: #f9c855;
}

button.warning:active {
    border: 1px solid #dea726;
    color: #dea726;
}





/* 危险按钮 */

button.danger:hover {
    border-color: #ff6d6d;
    color: #ff6d6d;
}

button.danger:active {
    border: 1px solid #e64242;
    color: #e64242;
}







/* 信息按钮 */

button.info:hover {
    border-color: #73ccff;
    color: #73ccff;
}

button.info:active {
    border: 1px solid #48ace6;
    color: #48ace6;
}
</style>
<script>
export default {

}
</script>