# 事件（逐步完善中）

| 事件                | 翻译                    | 说明                                  |
| ------------------- | ----------------------- | ------------------------------------- |
| Action              | 动作                    | 和属性中的一样                        |
| ActiveControl       | 默认控件                | 和属性中的一样                        |
| Constraints         | 限制条件                | 和属性中的一样                        |
| Menu                | 菜单                    | 和属性中的一样                        |
| OnActivate          | 激活时执行              | 程序被激活时                          |
| OnChangeBounds      | 变更边界                | 移动窗体，修改大小都会激活            |
| OnClick             | 点击时执行              | *                                     |
| OnClose             | 关闭时执行              | *                                     |
| OnCloseQuery        | 关闭请求时执行          | 此事件优先于OnClose                   |
| OnConstrainedResize | 调整时执行              | 窗体移动，修改大小                    |
| OnContextPopup      | 右键请求PopupMenu时执行 | 即使没有PopupMenu依旧会执行           |
| OnCreate            | 创建时执行              | *                                     |
| OnDbClick           | 双击时执行              | *                                     |
| OnDeactivate        | 取消激活状态时执行      | 也就是停用的时候激活                  |
| OnDestroy           | 销毁时执行              | *                                     |
| OnDockDrop          | 停靠释放时执行          |                                       |
| OnDockOver          | 停靠经过时执行          |                                       |
| OnDragDrop          | 拖动释放                |                                       |
| OnDragOver          | 拖动经过                |                                       |
| OnDropFiles         | 拖放文件后执行          |                                       |
| OnEndDock           | 停靠完成后执行          |                                       |
| OnGetSiteInfo       | 获得锚点信息时执行      |                                       |
| OnHelp              | 帮助按键时执行          | F1                                    |
| OnHide              | 隐藏时执行              | *                                     |
| OnKeyDown           | 按键按下时执行          |                                       |
| OnKeyPress          | 按键时执行              |                                       |
| OnKeyUP             | 按键弹起时执行          |                                       |
| OnMouseDown         | 鼠标按下时执行          |                                       |
| OnMouseEnter        | 鼠标进入控件范围时执行  |                                       |
| OnMouseLeave        | 鼠标离开控件方位时执行  |                                       |
| OnMouseMove         | 鼠标移动时执行          |                                       |
| OnMouseUp           | 鼠标弹起时执行          |                                       |
| OnMouseWheel        | 鼠标滚轮滚动时执行      |                                       |
| OnMouseWheelDown    | 滚轮向下时执行          |                                       |
| OnMouseWheelHorze   | 滚轮横向滚动时执行      |                                       |
| OnMouseWheelLeft    | 滚轮向左时执行          |                                       |
| OnMouseWheelRight   | 滚轮向右时执行          |                                       |
| OnMouseWheelUp      | 滚轮向上时执行          |                                       |
| OnPaint             | 重绘界面时执行          | *鼠标经过或者界面有变化都会绘制一次   |
| OnResize            | 调整大小时执行          | *启动时也算一次，因此正常后再进行判断 |
| OnShortCut          | 按键时执行              | *按下和弹起各算一次                   |
| OnShow              | 显示时执行              | *                                     |
| OnShowHint          | 显示提示信息时执行      |                                       |
| OnStartDock         | 开始停靠时执行          |                                       |
| OnUnDock            | 未停靠时执行            |                                       |
| OnUTF8KeyPress      | UTF8按键时执行          | win10下我们的按键就是UTF8             |
| OnWindowStateChange | 窗体状态变化时执行      | *                                     |
| PopupMenu           |                         | 和属性中的一样                        |
| PopupParent         |                         | 和属性中的一样                        |

