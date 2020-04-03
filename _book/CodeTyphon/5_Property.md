# 属性(此处会逐步完善)

属性默认显示正常字体，如果修改对应属性不是默认值，对应字体就变为粗体

| 属性                 | 翻译         | 参数 | 配套控件   | 配套事件  | 说明                         |
| -------------------- | ------------ | ------ | ---------- | --------- | ---------------------------- |
| Action               | 动作         |      | ActionList |           | * 选择ActionList中的动作执行 |
| ActiveControl        | 激活控件     |      |            |           | 默认激活的控件               |
| align                | 对齐方式     |      |            |           | Form中无效，控件中常用属性   |
| AllowDropFiles       | 允许拖放文件 | True/False |            | DropFiles |                              |
| AlphaBlend           | Alpha透明 | True/False |            |           | 打开Alpha透明 |
| AlphaBlendvalue      | Alpha透明值 | 0-255 |            |           | 确定窗体的透明度 0-255 |
| Anchors              | 锚点 |  |            |           | 用来确定控件的对齐 |
| AutoScroll           | 自动滚动 | True/False |            |           | 根据窗口自动生成滚动条 |
| AutoSize             | 自动大小 | True/False |            |           | 根据内容自动调整大小 |
| BiDiMode             |              |      |            |           | 为从右向左写的语言提供支持 |
| BorderIcons          | 边框图标 |      |            |           |                              |
| BorderStyle          | 边框形状(样式) |  |            |           |                              |
| BorderWidth          | 边框宽度 |      |            |           |                              |
| Caption              | 标题/文字内容 |      |            |           |                              |
| ChildSizing          |              |      |            |           |                              |
| Color                | 颜色 |      |            |           | 一般为窗体或者控件的可见颜色 |
| Constraints          | 限制条件 |      |            |           |                              |
| Cursor               | 光标 |      |            |           | 光标在窗体或者空间上的光标形状 |
| DefaultMonitor       | 默认显示器 |      |            |           | 程序显示在哪个默认显示器上 |
| DesignTimePPI        | 设计时间PPI |      |            |           | 写程序的时候的PPI |
| DockSite             | 锚点 | True/False |            |           |                              |
| DoubleBuffered       | 双重缓冲 | True/False |            |           | 重要用来解决有时候程序闪烁的问题 |
| DragKind             |              |      |            |           |                              |
| DragMode             |              |      |            |           |                              |
| Enabled              | 可用 | True/False |            |           | 控件或窗体是否可用，不可用为灰色 |
| FocusControl | 焦点控件 |  | TLabel | | Label中包含 &M，就代表按下Alt+M后，FocusControl中选择的控件即获得焦点 |
| Font                 | 字体 |      |            |           |                              |
| FormStyle            | 窗体样式 |      |            |           | 设置窗体类型以及最前显示 |
| Height               | 高度 |      |            |           | 窗体或控件的高度 |
| HelpContext          | 帮助ID号 |      |            |           |                              |
| HelpFile             | 帮助文件 |      |            |           |                              |
| HelpKeyword          | 帮助关键词 |      |            |           |                              |
| HelpType             | 帮助类型 |      |            |           |                              |
| Hint                 | 提示信息 |      |            |           | 必须 ShowHint打开才可显示 |
| HorzScrollBar        | 横向滚动条 |      |            |           |                              |
| Icon                 | 图标 |      |            |           | Form标题栏的图标 |
| KeyPreview           | 按键预览 |      |            |           | 指定此窗体是否需在目前的ACTIVE组件之前取得键盘输入 |
| Left                 | 左边距 |      |            |           |                              |
| Menu                 | 菜单 |      | TMainMenu |           |                              |
| Name                 | 名称 | Text |            |           |                              |
| ParentBiDiMode       |              | True/False |            |           |                              |
| ParentDoubleBuffered |              | True/False |            |           |                              |
| ParentFont           | 父字体 | True/False |            |           |                              |
| Picture | 图片 |  | TImage ... | | 包含图片类控件的图片选择 |
| PixelsPerInch        |              |      |            |           |                              |
| PopupMenu            | 弹出菜单 |      | TPopupMenu |           | 右键菜单 |
| PopupMode            | 弹出模式 |      |            |           |                              |
| PopupParent          |              |      |            |           |                              |
| Position             |              |      |            |           |                              |
| Proportional | 锁定比例 | | | | 缩放的时候按照比例缩放，需要Stretch属性开启 |
| Scaled               | 缩放比例 | True/False |            |           |                              |
| SessionProperties    | 会话属性 |      |            |           |                              |
| ShowHint             | 显示提示 | True/False |            |           | 鼠标放在窗体或者空间上显示Hint中的内容 |
| ShowInTaskBar        | 任务栏显示 |      |            |           |                              |
| Stretch | 延伸/缩放 | | TImage ... | | 按照控件大小自动缩放 |
| StretchInEnabled | 延伸缩小开启 | | TImage ... | |  |
| StretchOutEnabled | 延伸放大开启 | | TImage ... | |  |
| Tag                  | 标签 |      |            |           |                              |
| Top                  | 高度 |      |            |           | 对应顶部的高度 |
| Transparent | 透明 | | | | 控件透明 |
| UseDockManager       | 使用停靠管理器 | True/False |            |           |                              |
| VertScrollBar        |              |      |            |           |                              |
| Visible              | 可见性 | True/False |            |           |                              |
| Width                | 宽度 |      |            |           | 窗体或者控件的宽度 |
| WindowState          | 窗口显示状态 |      |            |           | 最大化/最小化/全屏 |

