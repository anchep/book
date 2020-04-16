# While语句

While循环语法

```pascal
while (condition) do S;
//如下
while number > 0 do
begin
   sum := sum + number;
   number := number -2;
end;

```

While是先判断，然后执行，一般两种方式退出while

1. 代码里面对while判断的参数进行修改，逐步超出while范围就退出了
2. 在while内部判断，然后使用break或者其他语句退出,这里简易break

流程图

![pascal while do loop](34_While/pascal_while_do_loop.jpg)

官方样例

```pascal
program whileLoop;
var
   a: integer;
begin
   a :=10;
   while  a<20  do
   begin
      writeln('value of a: ', a);
      a := a +1;
  end;
end.
```

运行结果

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
```

