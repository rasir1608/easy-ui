<template>
    <div>
        <div class="radio-group style-radios">
            <label v-for="(item,index) in radioData" :key="index" :for="'radio'+index" :class="[isChecked === index || isCheckedDisabled.indexOf(index) !== -1?'is-checked':'',isDisabled.indexOf(index) !== -1 || isCheckedDisabled.indexOf(index) !== -1?'disabled':'']" @click="checkRadio(item,index)">
                <input type="radio" :id="'radio'+index" name="radio" :disabled="isDisabled.indexOf(index) !== -1 || isCheckedDisabled.indexOf(index) !== -1">
                <span>{{item}}</span>
            </label>
        </div>
    </div>
</template>
<style scoped>
.radio-group.style-radios {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    background: #ffffff;
    font-size: 14px;
}

.radio-group.style-radios label {
    display: flex;
    cursor: pointer;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    position: relative;
    padding: 10px;
    border: 1px solid #20a0ff;
    border-right: 0;
    transition: all 0.2s linear;
}

.radio-group.style-radios label input {
    cursor: pointer;
}

.radio-group.style-radios label.disabled input {
    cursor: not-allowed;
}

.radio-group.style-radios label:first-of-type {
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
}

.radio-group.style-radios label:last-of-type {
    border-top-right-radius: 5px;
    border-bottom-right-radius: 5px;
    border: 1px solid #20a0ff;
}

.radio-group.style-radios label.disabled {
    color: #ccc;
}

.radio-group.style-radios label.disabled.is-checked {
    background: #EEF1F6;
    color: #ccc;
}

.radio-group.style-radios label.is-checked {
    color: #ffffff;
    background: #20a0ff;
}

.radio-group.style-radios label input[type='radio'] {
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
            radioData: ['备选项1', '备选项2', '备选项3', '备选项4', '备选项5'],
            isDisabled: [0, 2],
            isCheckedDisabled: [0, 3],
        }
    },
    methods: {
        checkRadio(item, index) {
            if (this.isDisabled.indexOf(index) !== -1 || this.isCheckedDisabled.indexOf(index) !== -1) return;
            this.isChecked = index;
        }
    }
}
</script>