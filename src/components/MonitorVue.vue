<template>
    <div id="demo">{{fullName}}</div>
</template>

<script>
export default {
    el:'#demo',
    data(){
        return{
            firstName:'Foo',
            lastName:'Bar',
            // fullName:'Foo Bar'
        }
    },
    // Watch:{
    //     firstName:function(val){
    //         this.fullName=val+''+this.lastName
    //     },
    //     lastName:function(val){
    //         this.fullName=this.firstName+''+val
    //     }
    // }
    computed:{
        fullName:function(){
            return this.firstName+' '+this.lastName
        }
    }
}
</script>