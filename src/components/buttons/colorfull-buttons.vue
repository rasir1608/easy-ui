<template>
    <div>
        <button class="success">成功按钮</button>
        <button class="warning">警告按钮</button>
        <button class="danger">危险按钮</button>
        <button class="info">信息按钮</button>
    </div>
</template>
<style scoped>
button {
    padding: 10px 20px;
    outline: 0;
    border-radius: 4px;
    cursor: pointer;
}

/* 成功按钮 */
button.success {
    background: #13ce66;
    border: 1px solid #13ce66;
    color: #fff;
}

button.success:hover {
    background: #42d885;
    border-color: #42d885;
}

button.success:active {
    background: #11b95c;
    border: 1px solid #11b95c;
}

/* 警告按钮 */
button.warning {
    background: #f7ba2a;
    border: 1px solid #f7ba2a;
    color: #fff;
}

button.warning:hover {
    background: #f9c855;
    border-color: #f9c855;
}

button.warning:active {
    background: #dea726;
    border: 1px solid #dea726;
}
/* 危险按钮 */

button.danger {
    background: #ff4949;
    border: 1px solid #ff4949;
    color: #fff;
}

button.danger:hover {
    background: #ff6d6d;
    border-color: #ff6d6d;
}

button.danger:active {
    background: #e64242;
    border: 1px solid #e64242;
}



/* 信息按钮 */

button.info {
    background: #50bfff;
    border: 1px solid #50bfff;
    color: #fff;
}

button.info:hover {
    background: #73ccff;
    border-color: #73ccff;
}

button.info:active {
    background: #48ace6;
    border: 1px solid #48ace6;
}

</style>
<script>
export default {

}
</script>