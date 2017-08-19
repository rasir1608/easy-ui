<template>
    <div>
        <div class="radio-group">
            <label for="radio1" :class="isChecked == 0?'is-checked':''" @click="checkRadio(0)">
                <div class="radio">
                    <span></span>
                    <input type="radio" id="radio1" name="radio">
                </div>
                <span>备选项1</span>
            </label>
            <label for="radio2" :class="isChecked == 1 ?'is-checked':''" @click="checkRadio(1)">
                <div class="radio">
                    <span></span>
                    <input type="radio" id="radio2" name="radio">
                </div>
                <span>备选项2</span>
            </label>
        </div>
    </div>
</template>
<style scoped>
.radio-group {
    display: flex;
    justify-content: center;
    align-items: center;
}

.radio-group label {
    display: flex;
    cursor: pointer;
    justify-content: center;
    align-items: center;
    margin: 5px;
}

.radio-group label.is-checked .radio span {
    border-width: 5px;
}

.radio-group label .radio {
    display: inline-block;
    position: relative;
    width: 15px;
    height: 15px;
    background: #fff;
    border-radius: 50%;
    overflow: hidden;
    margin-right: 5px;
}

.radio-group label .radio span {
    display: block;
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    border-radius: 50%;
    border: 1px solid #20a0ff;
    box-sizing: border-box;
    z-index: 1;
    margin: 0;
    padding: 0;
    transition: all 0.1s linear;
}

.radio-group label input[type='radio'] {
    width: 100%;
    height: 100%;
    opacity: 0;
    position: absolute;
    left: 0;
    top: 0;
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    z-index: 2;
}
</style>
<script>
export default {
    data() {
        return {
            isChecked: -1
        }
    },
    methods:{
        checkRadio(index){
            this.isChecked = index;
        }
    }
}
</script>