# With 语句

With 语法

```
with Memo1.lines do
begin
	add('text');
end;
```

With 主要就是用来快速处理控件内容的，相比传统每次书写控件名称要简洁很多。

代码样例

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
    Button2: TButton;
    Memo1: TMemo;
    procedure Button1Click(Sender: TObject);
    procedure Button2Click(Sender: TObject);
    procedure FormCreate(Sender: TObject);
  private

  public

  end;

var
  Form1: TForm1;

implementation

{$R *.frm}

{ TForm1 }

procedure TForm1.FormCreate(Sender: TObject);
begin

end;

procedure TForm1.Button1Click(Sender: TObject);
var
  i: integer;
begin
  Memo1.Clear;
  for i := 0 to 10 do
  begin
    Memo1.Left := 10;
    Memo1.Top := 10;
    Memo1.Lines.Add('Num.' + i.tostring);
  end;
end;

procedure TForm1.Button2Click(Sender: TObject);
var
  i:integer;
begin
  Memo1.Clear;
  with Memo1 do         //内部的代码就可以省掉 Memo1.
  begin
    Left := 15;
    Top := 15;

    for i:=0 to 9 do lines.Add('WithNun.'+i.tostring);
  end;

end;

end.

```

