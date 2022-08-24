<template>
    <ul id="example-1">
        <li v-for="item in items" :key="item.message">
        {{item.message}}
        </li>
    </ul>
</template>
<script>
export default {
    el:'#example-1',
    data(){
        return{
            items:[
                {message:'Foo'},
                {message:'Bar'},
            ],
            sets:[[1,2,4,5],[8,6,9]]
        }
    },
    methods:{
        even:function(numbers){
            return numbers.filter(function(number){
                return number%2===0
            })
        }
    }
}
</script>