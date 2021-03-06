#app 产品版本号定义

>分三项：

`<主版本号>.<次版本号>.<修订版本号>，如 1.0.0。`

>修改规则：（除 **修订版本号** 的改变由开发人员自己制定外，**主版本号，次版本号** 由产品经理协助制定）

    主版本号：产品功能模块有大的变动，比如增加多个模块或者整体架构发生变化。

    次版本号：和主版本相对而言，次版本号的升级对应的只是局部的变动。但该局部的变动造成了程序和以前版本不能兼容，或者对该程序以前的协作关系产生了破坏，或者是功能上有大的改进或增强。

    修订版本号：局部的变动，主要是局部函数的功能改进，或者bug的修正，或者功能的扩充。
    
>版本号管理策略

    1．项目未发布时时，版本号为 0.1 或 0.1.0;
    2．当项目在进行了局部修改或 bug 修正时，主版本号和子版本号都不变，修正版本号加 1;
    3．当项目在原有的基础上增加了部分功能时，主版本号不变，子版本号加 1，修正版本号复位为 0，因而可以被忽略掉 ;
    4．当项目在进行了重大修改或局部修正累积较多，而导致项目整体发生全局变化时，主版本号加 1;
    5．另外，编译版本号一般是编译器在编译过程中自动生成的，我们只定义其格式，并不进行人为控制 .

**注意：**

    每项必须为 0 或者 正整数，数字前不要用0做前缀。2.1.6 是合适的，而 2.1.06 就匪夷所思，不合适。
