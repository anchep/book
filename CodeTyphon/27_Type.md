









# Type数据类型

数据类型是日常需要考虑的一个很重要的问题，我们写代码的就是为了更为方便的操作数据，所以对数据的类型要求极为重要。

Pascal语言对于数据的类型检查严格，类型不匹配的统一不处理，但是可以通过类型转换转换为需要的数据类型。

#### 数据类型分为：标准数据类型；高级数据类型

1. 标准数据类型：就是系统里面已经定义的数据类型
2. 高级数据类型：其实就是自己定义的数据类型

|              |                                                              |                                                              |                                                   |                           |              |            |
| ------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------- | ------------------------- | ------------ | ---------- |
| 分类         | 范围                                                         | 字节                                                         | 备注                                              |                           |              |            |
| 简单类型     | 序数                                                         | 整数                                                         | Integer                                           | -2147483648 .. 2147483647 | 4            | 有符号32位 |
| Cardinal     | 0 .. 4294967295                                              | 4                                                            | 无符号32位                                        |                           |              |            |
| Shortint     | -128 .. 127                                                  | 1                                                            | 有符号8位                                         |                           |              |            |
| Smallint     | -32768 .. 32767                                              | 2                                                            | 有符号16位                                        |                           |              |            |
| Longint      | -2147483648 .. 2147483647                                    | 4                                                            | 有符号32位                                        |                           |              |            |
| Int64        | -263 .. 263                                                  | 8                                                            | 有符号64位                                        |                           |              |            |
| Byte         | 0 .. 255                                                     | 1                                                            | 无符号8位                                         |                           |              |            |
| Word         | 0 .. 65535                                                   | 2                                                            | 无符号16位                                        |                           |              |            |
| Longword     | 0 .. 4294967295                                              | 4                                                            | 无符号32位                                        |                           |              |            |
| 字符         | AnsiChar(Char)                                               | ANSI字符集                                                   |                                                   | 8位                       |              |            |
| WideChar     | Unicode字符集                                                |                                                              | 16位                                              |                           |              |            |
| 布尔         | Boolean                                                      | False < True Ord(False) = 0 Ord(True) = 1 Succ(False) = True Pred(True) = False | 1                                                 |                           |              |            |
| ByteBool     | False <> True Ord(False) = 0 Ord(True) <> 0 Succ(False) = True Pred(False) = True | 1                                                            |                                                   |                           |              |            |
| WordBool     | 2                                                            |                                                              |                                                   |                           |              |            |
| LongBool     | 4                                                            |                                                              |                                                   |                           |              |            |
| 枚举         |                                                              |                                                              |                                                   |                           |              |            |
| 子界         |                                                              |                                                              |                                                   |                           |              |            |
| 实数         |                                                              | Real                                                         | 5.0×10-324 .. 1.7×10308                           | 8                         | [精度]15..16 |            |
| Real48       | 2.9×10-39 .. 1.7×1038                                        | 6                                                            | [精度]11..12; 向后兼容                            |                           |              |            |
| Single       | 1.5×10-45 .. 3.4×1038                                        | 4                                                            | [精度]7..8                                        |                           |              |            |
| Double       | 5.0×10-324 .. 1.7×10308                                      | 8                                                            | [精度]15..16                                      |                           |              |            |
| Extended     | 3.6×10-4951 .. 1.1×104932                                    | 10                                                           | [精度]19..20                                      |                           |              |            |
| Comp         | -263 + 1 .. 263 - 1                                          | 8                                                            | [精度]19..20                                      |                           |              |            |
| Currency     | -922337203685477.5808 ..  922337203685477.5807               | 8                                                            | [精度]19..20                                      |                           |              |            |
| 字符串       |                                                              |                                                              | ShortString                                       | 255个字符                 | 2..256B      | 向后兼容   |
| AnsiString   | 大约 231 个字符                                              | 4B..2GB                                                      | 8位(ANSI)字符                                     |                           |              |            |
| WideString   | 大约 230 个字符                                              | 4B..2GB                                                      | 多用户服务和 多语言应用程序;  和com定义的BSTR兼容 |                           |              |            |
| 其他         | String String[0..255] PChar PAnsiString PWideString          |                                                              |                                                   |                           |              |            |
| 结构类型     | 集合                                                         |                                                              | Set                                               | 最多256个元素[0..255]     |              |            |
| 数组         | 静态数组                                                     |                                                              |                                                   |                           |              |            |
| 动态数组     |                                                              |                                                              |                                                   |                           |              |            |
| 记录         |                                                              | Record                                                       |                                                   |                           |              |            |
| 文件         |                                                              | File                                                         |                                                   |                           |              |            |
| 类           |                                                              | Class                                                        |                                                   |                           |              |            |
| 类引用       |                                                              | Class reference                                              |                                                   |                           |              |            |
| 接口         |                                                              | Interface                                                    |                                                   |                           |              |            |
| 指针类型     | 无类型指针                                                   |                                                              | Pointer                                           |                           |              |            |
| 有类型指针   | 预定义类型指针                                               | PAnsiString PString PByteArray PCurrency PDouble PExtended PSingle PInteger POleVariant PShortString PTextBuf PVarRec PVariant PWideString PWordArray |                                                   |                           |              |            |
| 过程类型     | 程序过程类型                                                 |                                                              | Procedural                                        |                           |              |            |
| 对象过程类型 |                                                              | Procedural                                                   |                                                   |                           |              |            |
| 变体类型     |                                                              |                                                              | Variant                                           |                           |              |            |
|              | OleVariant                                                   |                                                              |                                                   |                           |              |            |

##### 数据类型之间的转换

| 例程           | 作用                                                         |
| -------------- | ------------------------------------------------------------ |
| Chr            | 将一个有序数据转换为一个ANSI字符                             |
| Ord            | 将一个有序类型值转换为它的序号                               |
| Round          | 转换一个实型值为四舍五入后的整型值                           |
| Trunc          | 转换一个实型值为小数截断后的整型值                           |
| Int            | 返回浮点数的整数部分                                         |
| IntToStr       | 将数值转换为字符串                                           |
| IntToHex       | 将数值转换为十六进制数字符串                                 |
| StrToInt       | 将字符串转换为一个整型数，如字符串不是一个合法的整型将引发异常 |
| StrToIntDef    | 将字符串转换为一个整数，如字符串不合法返回一个缺省值         |
| Val            | 将字符串转换为一个数字（传统Turbo Pascal例程用于向后兼容）   |
| Str            | 将数字转换为格式化字符串（传统Turbo Pascal例程用于向后兼容） |
| StrPas         | 将零终止字符串转换为Pascal类型字符串，在32位Delphi中这种类型转换是自动进行的 |
| StrPCopy       | 拷贝一个Pascal类型字符串到一个零终止字符串, 在32位Delphi中这种类型转换是自动进行的 |
| StrPLCopy      | 拷贝Pascal类型字符串的一部分到一个零终止字符串               |
| FloatToDecimal | 将一个浮点数转换为包含指数、数字及符号的十进制浮点记录类型   |
| FloatToStr     | 将浮点值转换为缺省格式的字符串                               |
| FloatToStrF    | 将浮点值转换为特定格式的字符串                               |
| FloatToText    | 使用特定格式，将一个浮点值拷贝到一个字符串缓冲区             |
| FloatToTextFmt | 同上面例程，使用特定格式，将一个浮点值拷贝到一个字符串缓冲区 |
| StrToFloat     | 将一个Pascal字符串转换为浮点数                               |
| TextToFloat    | 将一个零终止字符串转换为浮点数                               |

以上转换方式在最新的ide中有更加简便的方式 .to模式，在IDE中只要输入到 . 然后稍等就会弹出对应的方法或者

例如：

```pascal
s:= '2';
  s:= s.ToInteger;       //这里就将【字符串类型的s】转换为【数字类型的s】
  s := s * 2;            //这里就可以将s 乘以 2 返回给 s    
```



#### 高级数据类型

###### 	枚举类型：例如每周的星期几就可以定义：

格式:　type 枚举类型标识符=(标识符1,标识符2,…,标识符n)

```pascal
type
  days=(sun,mon,tue,wed,thu,fri,sat);
  colors=(red,yellow,blue,white,black,green);
```

枚举类型中的参数不能相同，枚举类型的数据只能赋值操作，不能进行运算操作，

```Pascal
type
    days=(sun,mon,tue,wed,thu,fri,sat);
　　colors=(red,yellow,blue,white,black,green);
var
    color:colors;
　　 weekday:days;
　//则下面语句是合法的:
　weekday:=mon;
　if weekday=sun then write('rest');
　//而下面语句是不合法的:
    mon:=1;           //错把枚举值当成变量名；
    weekday:=blue；   //枚举值blue不属于枚举变量weekday的值域；
    read(color);      //枚举类型变量 不能用读语句进行赋值；
    write(weekday); writeln(blue);//不能通过写语句输出枚举类型的变量值和枚举值。
```

可以把变量的说明与类型的定义合并在一起，如:

```Pascal
  　　var
  　　    holiday,workday:(sun,mon,tue,wed,thu,fri,sat);
  　　　   color:(red,yellow,blue,white,black,green);
```

###### 	子界类型

type 子界类型标识符=常量1..常量2

```pascal
type  letter='a'..' z ';
    var ch1,ch2:letter;
```

可以合并成:

```pascal
var ch1,ch2:'a'..'d';
```

###### 	集合类型

集合类型的一般形式为： set of 基类型;集合中的数据无顺序

```pascal
  type
    numbers = set of 0..9;
    ch = set of char;
    day = (sun, mon, tue, wed, thu, fri, sat);
  var
    s: numbers;
    c: ch;
    weekday: day;
```

可以将类型说明与变量说明合并在一起，如:

```pascal
  var s:set of 0..9;                               { 子界型 }
      c:set of char;
      weekday: (sun,mon,tue,wed,thu,fri,sat);      { 枚举型 }
```