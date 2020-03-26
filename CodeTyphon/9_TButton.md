# TButton 按钮

1. ##### 添加Button控件到窗口

   ![](9_TButton/20.png)

2. ##### 调整按钮大小

   ![](9_TButton/21.png)

3. ##### Caption 修改按钮名称

   ![](9_TButton/22.png)

4. ##### Align 对齐：

   1. Align=alButtom

      ![](9_TButton/23.png)

   2. Align=alClient

      ![](9_TButton/24.png)

   3. Align=alCustom

      ![](9_TButton/25.png)

   4. Align=alLeft

      ![](9_TButton/26.png)

   5. Align=alNone(默认)

      ![](9_TButton/27.png)

   6. Align=alRight

      ![](9_TButton/28.png)

   7. Align=alTop

      ![](9_TButton/29.png)

5. ##### AutoSize 自动大小

   ![](9_TButton/30.png)

   ​	`选择AutoSize后，按钮会根据俺就中文字的长度和高度来自适应按钮的长度和高度`

6. ##### Cursor 光标形状

   ​	此处截图比较麻烦，设置为 crHandPoint ，鼠标移动到按钮上就会显示为手的形状

7. ##### Enable 可用/禁用

   ![](9_TButton/32.png)

   ​	显示效果：![](9_TButton/33.png)

8. ##### Font 字体

   1. 设置方式：![](9_TButton/34.png)
   2. 设置效果：![](9_TButton/35.png)

9. ##### Hint 提示信息 ShowHint

   1. 设置提示信息：![](9_TButton/36.png)
   2. 设置效果：![](9_TButton/37.png)

10. ##### Left & Top 左 和 上

    左和上用来确定按钮位置

11. ##### Height & Width 高度 和 宽度

    高度和宽度确定按钮大小

12. ##### Name 名字

    1. 控件的名字，日常命令操作的时候使用的就是这个名字

    2. 将按钮的Name 设置为 BtnMain ，然后在命令行中调用

    3. 命令：

       ```pascal
       BtnMain.Caption := '按钮名字';  
       ```

    4. 效果：

       ![](9_TButton/38.png)

13. ##### Visible 可见性

    1. 设置为True ：按钮可以看到
    2. 设置为False：按钮无法看到
    3. IDE界面：![](9_TButton/39.png)
    4. 运行效果：![](9_TButton/40.png)

