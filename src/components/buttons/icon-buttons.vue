<template>
    <div>
        <button class="primary loading">
            <i class="iconfont icon-jishi"></i>加载中
        </button>
        <button class="primary iconfont icon-writefill">
        </button>
        <button class="primary">
            <i class="iconfont icon-search"></i>搜索
        </button>
         <button class="primary">
            赞<i class="iconfont icon-appreciate_light"></i>
        </button>
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
    padding: 5px 10px;
}

/* 小型按钮 */
button.small{
    padding: 5px 10px;
}

/* 超小型按钮 */
button.mini{
    padding: 2px 5px;
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

button .iconfont{
    margin-right: 5px;
    margin-left: 5px;
}
button.loading .iconfont {
    display: inline-block;
    margin-right: 5px;
    animation: loading 1s linear infinite;
}

@keyframes loading {
    from {
        transform: rotate(0deg);
    }
    to {
        transform: rotate(360deg);
    }
}



/* button.loading::before {
    pointer-events: none;
    content: "";
    position: absolute;
    left: -1px;
    top: -1px;
    right: -1px;
    bottom: -1px;
    border-radius: inherit;
    background-color: hsla(0, 0%, 100%, .35);
} */
</style>
<script>
export default {

}
</script>