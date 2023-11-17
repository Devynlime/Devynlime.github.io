# Vue 图片切换器

这是一个使用 Vue.js 构建的图片切换器。用户可以点击按钮来切换显示的图片，每个图片都有一个对应的描述文字。

## 实现逻辑

在 HTML 中，我们有一个 Vue 应用的根元素，它的 id 是 `app`。在这个元素内部，我们有一个 `.content-container`，它包含了按钮和图片。

按钮是一个 `.button-container`，它包含了三个图片按钮。每个按钮都有一个 `v-on:click` 指令，当用户点击按钮时，它会改变 currentImage 的值。

图片是一个 `.image-container`，它包含了一个图片元素和三个 `.overlay` 元素。图片元素的 `src` 属性绑定到 `images[currentImage]`，所以当 `currentImage` 的值改变时，显示的图片也会改变。`.overlay` 元素是描述图片的文字，它们使用 `v-if` 指令来根据 `currentImage` 的值来显示或隐藏。

在 CSS 中，我们使用 Flexbox 布局来排列 `.content-container` 的子元素（即按钮和图片）。我们还使用了 CSS 动画来实现 `.overlay` 元素的闪烁效果。

## 使用方法

打开 `index.html` 文件在浏览器中查看效果。

点击按钮来切换图片。每个图片都有一个对应的描述文字，这个文字会在图片上方闪烁。

### 注意事项

确保你的浏览器支持 Vue.js 和 CSS 动画。
如果你想改变图片或描述文字，你需要修改 Vue 实例的 `data` 选项和 `.overlay` 元素的内容。
如果你想改变布局或样式，你需要修改 CSS 规则。