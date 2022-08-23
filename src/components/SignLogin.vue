<template >
    <!-- // 刚刚它提示说没有打开 模板template语法 的提示，按照它提示的打开了
    //怎么打开
    //这是干啥的
    // 就是在 template 内的智能提示功能
    //开不开有影响吗
    // 对编译没有啥影响，可能对写代码有影响吧，具体不知道
    // 哦，应该是jsx语法提示。这里没有用到，没啥影响。。去掉了蓝色波浪线主要是。
    //好吧 -->
    <div v-if="loginType==='username'">
    <label>Username</label>
    <input placeholder="请输入名字" key="username-input">
    </div>
    <div v-else>
        <label>Email</label>
        <input placeholder="请输入邮箱" key="email-input">
    </div>
</template>
<!-- <template v-else>
<lable>Email</lable>
</template> -->
<script>

export default {
    name: "SignLogin",
    data(){
      return {
        loginType: 'username'
      }
    },
    methods:{

    }
}
</script>