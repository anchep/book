# Constants and variables 常量和变量

#### 常量分为两种：一种系统的常量，一种自定义的常量

1. 系统常量即为一些日常的基本参数，如pi等
2. 自定义常量日常使用较多

使用Const来定义，常量会自动盘点自己的类型，因此不用指定数据类型。

```pascal
Const
  name1 = 'Houzi';
  name2 = 'taozi';
var
  Form1: TForm1;

implementation

{$R *.frm}

{ TForm1 }

procedure TForm1.Button1Click(Sender: TObject);
begin
  Edit1.Text:= name1;
  Edit2.Text:=name2;
end;    
```

最新的还有 ResourceString 此方式会将字符串保存到系统特定区域，有利于对程序进行多语言开发

```pascal
resourcestring
  AuthorName = 'Marco Cantù';
  BookName = 'Essential Pascal';

procedure TForm1.Button1Click(Sender: TObject);
begin
  ShowMessage (BookName + #13 + AuthorName);
end;
```



#### 变量：自定义可变的部分。

使用 Var定义

1. 变量一个要分清楚全局变量和私有变量
2. 变量如果冲突，优先取值私有变量

```pascal
unit Unit1;

{$mode objfpc}{$H+}

interface

uses
  Classes, SysUtils, Forms, Controls, Graphics, Dialogs, StdCtrls;

type

  { TForm1 }

  TForm1 = class(TForm)
    Button1: TButton;
    Edit1: TEdit;
    Edit2: TEdit;
    procedure Button1Click(Sender: TObject);
  private

  public

  end;

var
  Form1: TForm1;
  name3:string   //这里整个单元可用，而且其他调用了此单元的单元也可以使用

implementation

{$R *.frm}

{ TForm1 }

procedure TForm1.Button1Click(Sender: TObject);
var
  //此处变量仅在下面的begin和end之间有用
  //name:string;         //此处使用的系统属性的的名称，因此会报错
  name1,name2:string;
begin
  name :='name';
  name1 := 'zhangsan';
  //name2 := 'lisi';           //name2 未赋值，结果会显示空
  //变量在使用前必须复制，养成好习惯，否则程序出错不好找
  Edit1.Text:= name1;
  Edit2.Text:=name2;
end;

end.

```





