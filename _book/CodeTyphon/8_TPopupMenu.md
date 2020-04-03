# TPopupMenu 弹出菜单

> ​	右键菜单，常用菜单，日常开发中使用频率很高。

1. ##### 添加控件

   ![](8_TPopupMenu/16.png)

2. ##### 双击控件，配置菜单

   ![](8_TPopupMenu/17.png)

3. ##### 配置弹出菜单响应位置：

   ![](8_TPopupMenu/18.png)

   >   选择Form1，在PopupMenu属性中，下拉选择新添加的 PopupMenu1

4. ##### 【F9】 运行程序，在窗体上右键查看效果

   ![](8_TPopupMenu/19.png)

5. ##### 补充

   

   控制顶级窗体相对于Window的WS_POPUP样式的行为。

   该PopupMode属性控制顶层形式的行为相对于窗口的WS_POPUP风格。具有WS_POPUP样式的窗口在Z顺序中始终位于其“所有者”上方。您可以使用PopupMode结合属性与[PopupParent](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.PopupParent)属性，避免因背后显示在屏幕上的另一种形式了一个模态对话框挂起应用程序的外观。

   > **注意：**使用PopupMode属性类似于`fsStayOnTop`为[FormStyle](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.FormStyle)属性指定，但是可以更好地控制分层。

   该PopupMode属性被自动设置为`pmAuto`当[的ShowModal](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.ShowModal)方法被调用。但是，这将导致重新创建窗口句柄，这通常是不希望的。为了避免重新创建窗口句柄，可以在调用[ShowModal](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.ShowModal)方法之前（例如在设计时）将PopupMode属性显式设置为。 `pmAuto`

   对于非模式设计窗口（例如工具选项板和其他浮动工具窗口），将PopupMode属性设置`pmExplicit`为。这导致窗口始终保持在主窗体的顶部。如果是拼合设计（窗口停靠在主窗体中），则设计窗口保留在设计器顶部。

   > **注意：**对于未停靠的窗口，设计窗口将保留在主窗体上方，从而允许其他顶层窗体遮盖设计窗口。

   如果希望弹出窗口具有Delphi 8之前的行为（将上述[ShowModal](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.ShowModal)项除外），则将PopupMode属性设置为。 `pmNone`

   通过将[PopupParent](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.PopupParent)属性设置为显式的TCustomForm，可以强制窗体的Z排序并创建用户无法更改的“堆叠”外观。如果PopupMode属性为，`pmExplicit`而[PopupParent](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.PopupParent)为nil，则Application.MainForm隐式用作[PopupParent](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.PopupParent)。如果未分配Application.MainForm，则将Application.Handle用作[PopupParent](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.PopupParent)。如果PopupMode属性设置为`pmAuto`，则Screen.ActiveForm用作[PopupParent](http://docwiki.embarcadero.com/Libraries/Rio/en/Vcl.Forms.TCustomForm.PopupParent)。