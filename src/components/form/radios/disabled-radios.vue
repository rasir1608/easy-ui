<template>
    <div>
        <div class="radio-group">
            <label  v-for="(item,index) in radioData" :key="index" :for="'radio'+index" :class="[isChecked === index || isCheckedDisabled.indexOf(index) !== -1?'is-checked':'',isDisabled.indexOf(index) !== -1 || isCheckedDisabled.indexOf(index) !== -1?'disabled':'']" @click="checkRadio(item,index)">
                <div class="radio">
                    <span></span>
                    <input type="radio" :id="'radio'+index" name="radio" :disabled="isDisabled.indexOf(index) !== -1 || isCheckedDisabled.indexOf(index) !== -1">
                </div>
                <span>{{item}}</span>
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
.radio-group label.disabled .radio span {
    border-color: #cccccc;
}
.radio-group label.disabled {
    color:#ccc;
    cursor: not-allowed;
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
            isChecked: -1,
            radioData:['备选项1','备选项2','备选项3','备选项4','备选项5'],
            isDisabled:[0,2],
            isCheckedDisabled:[0,3],
        }
    },
    methods:{
        checkRadio(item,index){
            if(this.isDisabled.indexOf(index) !== -1 || this.isCheckedDisabled.indexOf(index) !== -1)return;
            this.isChecked = index;
        }
    }
}
</script>