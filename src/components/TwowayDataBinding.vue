<template>
    <div id="select">
        <select v-model="selected">
            <option disabled value="">请选择</option>
            <option>A</option>
            <option>B</option>
            <option>C</option>
        </select>
        <span>Selected:{{selected}}</span>
    </div>
    <div id="select2">
        <select v-model="selected2" multiple style="width:100px">
            <option disabled value="">请选择</option>
            <option>A</option>
            <option>B</option>
            <option>C</option>
        </select>
        <span>Selected:{{selected2}}</span>
    </div>
    <div id="components-demo">
        <button-counter></button-counter>
    </div>
</template>
<script>
export default {
    el:'select,components-demo',
    data(){
        return {
            selected:'',
            selected2:[]
        }
    }
}
</script>