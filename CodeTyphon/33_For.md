# For语句

#### For循环语法

```pascal
for:= to [down to] do 
   S;
   //如下
for i:=1 to 10 do writeln(i);
```

For循环注意运行次数，必须明确运行几次，才好处理其中的代码

必须使用整数

#### 流程图

![pascal for do loop](33_For/pascal_for_do_loop.jpg)

#### 官方样例

```pascal
program forLoop;
var
   a: integer;
begin
   for a :=10  to 20 do
   begin
      writeln('value of a: ', a);
   end;
end.
```

#### 运行结果

```pascal
value of a: 10
value of a: 11
value of a: 12
value of a: 13
value of a: 14
value of a: 15
value of a: 16
value of a: 17
value of a: 18
value of a: 19
value of a: 20
```

