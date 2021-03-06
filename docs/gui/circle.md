# 圆形 Circle

Circle 可绘制圆形

> 不设置 lineWidth 或 color 圆形不可见
> 画扇形时,暂时不支持同时设置边界和填充

## 属性

| 属性名 | 属性类型 | 默认值 | 说明 |
| --- | --- | --- | --- | --- |
| width | number | 0 | 圆直径为width/height小值 |
| height | number | 0 | 圆直径为width/height小值 |
| lineColor | number | 0xffffff | 设置边框颜色 |
| lineWidth | number | 0 | 设置边框宽度 |
| lineType | "full" , "dash" | "full" | 虚线or实线 |
| color | number | | 设置填充色 |
| fillAlpha | number | 1 | 设置填充透明度 |
| anchorX | 0-1 |  | 设置内部X坐标 |
| anchorY | 0-1 |  | 设置内部Y坐标 |
| startAngle | number |  | 起始角度 |
| endAngle | number |  | 终止角度 |

## 事件

| 事件名  | 说明 | 参数 |
| --- | --- | --- |

## 方法
| 函数名 | 参数 | 函数返回值 | 说明 |
| drawGraph |  |  | 绘制图形 |

## 样式

> [基础样式](/handbook/style.html#样式)

## 定义
``` typescript
const circle: gui.Circle = {
    name: "circle",
    type: guiType.Circle,
    color:0xffffff,
    lineColor: 0xff00cc,
    lineWidth: 1,
    width:100
};
```

## 使用
``` typescript
{
id: "circle",
libId: ComponentId.circle,
}
```

## 示例

> 可点击左上角菜单，查看其他定义类

<iframe
     src="https://codesandbox.io/embed/circle-pk7rs?fontsize=14&hidenavigation=1&module=%2Fsrc%2Fcomponents.ts&theme=dark"
     style="width:100%; height:720px; border:0; border-radius: 4px; overflow:hidden;"
     title="circle"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>