<template>
    <div id="watch-example">
        <p>
            Ask a yes/no question:
            <input v-model="question">
        </p>
        <p>{{answer}}</p>
    </div>
</template>
<script>

export default {
    el:'#watch-example',
    data(){
        return{
            question:'',
            answer:'I cannot give you an answer until you ask a question!'
        }
    },
    // watch:{
    //     question:function(newQuestion,oldQuestion){
    //         this.answer='waiting for you to stop typing...'
    //         this.debouncedGetAnswer()
    //     }
    // },
    // created:function(){
    //     this.debouncedGetAnswer=_.debounce(this.debouncedGetAnswer,500)}, 
    // methods:{
    //     getAnswer:function(){
    //         if(this.question.indexOf('?')===-1){
    //             this.answer='Questions usually contain a question mark.;-)'
    //             return 
    //         }
    //         this.answer='Tinking...'
    //         var vm=this
    //         axios.get('https://yesno.wtf/api')
    //         .then(function(response){
    //             vm.answer=_.capitalize(response.data.answer)
    //         })
    //         .catch(function(error){
    //             vm.answer='Error! Could not reach the API.'+error
    //         })
    //     }
    // }
}
</script>