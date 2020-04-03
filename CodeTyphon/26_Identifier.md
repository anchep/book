# Identifier标识符

标识符是Pascal语言的基础。

#### 常用标识符：

var:变量

Const:常量

Type:类型

Procedure:过程

Function:函数

Method:方法

Unit:单元

#### 标识符分为三类：标注标识符；自定义标识符；限定标识符。

##### 标准标识符：这些带定义变量的时候是不能使用的。

1. 常量：False / True / cdGrayed等
2. 类型：Boolean  Integer Char 等
3. 函数：Cos，Sin，Abs等
4. 过程：get，put，new等
5. 文件：input，output等

##### 自定义标识符：自定义标识符是我们开发中最常用的，一定要避免和标准标识符冲突。

1. 不能带空格
2. 不区分大小写
3. 只能字符或者下划线开头
4. 不要超过225个字符
5. 就是不能使用标准标识符或者其他系统预留的功能以及函数作为自定义标识符名称

##### 限定标识符：用来限定某一个单元，然后调用单元内部的方法或者函数

例如：

```pascal
var
a:real;
a:=system.cos(pi);
```

#### 系统保留字，这里其实就是pascal语言默认使用的一些标识符。

例如：and if then with 等日常编辑软件中使用的一些命令

| and            | array          | as          | asm        | begin          | case    |
| -------------- | -------------- | ----------- | ---------- | -------------- | ------- |
| class          | const          | constructor | destructor | dispinterface  | div     |
| do             | downto         | else        | end        | except         | exports |
| file           | finalization   | finally     | for        | function       | goto    |
| if             | implementation | in          | inherited  | initialization | inline  |
| interface      | is             | label       | library    | mod            | nil     |
| not            | object         | of          | or         | out            | packed  |
| procedure      | program        | property    | raise      | record         | repeat  |
| resourcestring | set            | shl         | shr        | string         | then    |
| threadvar      | to             | try         | type       | unit           | until   |
| uses           | var            | while       | with       | xor            |         |

#### 指令符：程序一般会默认生成的，命名的时候也要避开

Object Pascal中规定的指令符有39个
说明：指令符private、protected、public、published和automated在定义对象类型时也作为保留字，而在其他场合则作为指令符。

#### 注释：注释分为可读性和可维护性

1. 组合1：两个大括号包含的部分  { 这里是注释 }  //必须成对出现，一一对应，不能嵌套
2. 组合2：两个单括号和星号组成的   (* 这里是注释 *)
3. 单符号： 两个斜杠后面的部分   //这里是注释
4. { 或者 (*  后面紧跟$ 表示是编译指令，这种主要用来处理编译过程中的一些内容，此类内容新手勿碰

由于上面部分理解起来比较困难，因此后面分开介绍具体代码操作