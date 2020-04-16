# Goto 语句

语法

```
goto label;
   ...
   ...
label: statement;
```

流程图

![cpp goto statement](39_ExitAbort/cpp_goto_statement.jpg)

官方样例

```pascal
program exGoto;
label 1; 
var
   a : integer;
begin
   a :=10;
   (* repeat until loop execution *)
   1: repeat
      if( a =15 )then
      begin
         (* skip the iteration *)
         a := a + 1;
         goto 1;
      end;
      writeln('value of a: ', a);
      a:= a + 1;
   until a = 20;
end.
```

运行结果

```pascal
value of a: 10
value of a: 11
value of a: 12
value of a: 13
value of a: 14
value of a: 16
value of a: 17
value of a: 18
value of a: 19
```

