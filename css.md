## css3的新样式

#### 1.弹性盒布局

Flex（Flexible Box）

align纵向排布

```css
display:flex

flex-grow/flex-shrink(如果空间足够就自动生长/如果空间不够就自动缩小 保持在父容器里)
```

#### 2.网格布局

与弹性盒类似，但是是二维的。但是个别浏览器不兼容。

```css
display:grid;
grid-template-columns:33% 33% 33%; //对列进行排布
grid-template-rows:33% 33% 33%; //对行进行排布

容器内部子div
place-self指定子元素如何布局
e.g.:
place-self:center;
```

### 2.11移动设备优先

在元数据标记中设置视口（viewpoint），可使得网页更适合移动端展示。(仅在移动端有效)

图形画在视口里，视口在窗口里。

视口以窗口的左下角为原点，根据参数进行布局。

```css
<meta name = "viewpoint" content = "width = device-width, initial-scale = 1">

initial-scale表示初始比例（视口像素和屏幕像素的比例）
initial-scale = 1 表示一个视口像素对应一个屏幕像素
initial-scale = 0.5 表示一个视口像素对应1/4个屏幕像素

width指定视口的宽度

user-scalable=no;表示不允许用户对视口进行放大

还有一些属性：
maximum-scale/minimum-scale（视口的最大最小值）
height(一般没人设置)
```

