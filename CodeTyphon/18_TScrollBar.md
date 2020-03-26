# TScrollBar 滚动条

> 老式滚动条，用处还是不少的。

1. 添加控件

   ![](18_TScrollBar/67.png)

2. 控件属性

   ![](18_TScrollBar/68.png)

   ![image-20200326195813441](18_TScrollBar/image-20200326195813441.png)

3. 运行效果

   ![](18_TScrollBar/69.png)

4. 示例代码

   1. ```pascal
      procedure TForm1.ScrollBar1Change(Sender: TObject);
      begin
        Edit1.Text:= ScrollBar1.Position.ToString;
      end; 
      ```

      

5. 补充