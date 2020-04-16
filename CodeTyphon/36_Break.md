# Break 语句

#### Break主要作用：

1. 强制退出最近的一层循环（注意：只能放在循环里；而且是只能跳出最近的一层循环），用于从for、while、repeat语句中强制退出
2. 终止case语句中的case

#### 终止循环-流程图

![cpp break语句](36_Break/cpp_break_statement.jpg)



#### 官方样例

```pascal
program exBreak;
var
   a: integer;
begin
   a :=10;
   while (a<20) do
    begin
      writeln('value of a: ', a);
      a:=a +1;
      if (a>15) then
       break; {terminate the loop}
    end;   
end.
```

#### 输出结果

```pascal
value of a: 10
value of a: 11
value of a: 12
value of a: 13
value of a: 14
value of a: 15
```

