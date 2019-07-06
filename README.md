# BookmarksBeautify
将浏览器书签美化，便于上传网络分享给他人。

![](https://raw.github.com/MoXiaoCC/BookmarksBeautify/master/img/1.png)

**该样式支持谷歌浏览器75.0.3770.100、chrome内核的edge和IE浏览器11导出的书签。**

**第一步**
导出书签

![](https://raw.github.com/MoXiaoCC/BookmarksBeautify/master/img/3.png)
![](https://raw.github.com/MoXiaoCC/BookmarksBeautify/master/img/2.png)
**第二步**
在`<TITLE>Bookmarks</TITLE>`后面插入

```html
<base target="_blank" /><!-- 所有链接新窗口打开 -->
<link rel="stylesheet" href="https://cdnjs.loli.net/ajax/libs/mdui/0.4.2/css/mdui.min.css"><!-- 引入MDUI css -->
<script src="https://cdnjs.loli.net/ajax/libs/mdui/0.4.2/js/mdui.min.js"></script><!-- 引入MDUI JS -->
<style>
body{max-width:1200px;margin:auto;}/* 所有连接新窗口打开 */
a{  text-decoration:none;
	display:inline-block;
	color:#233333;
	float:left;
	width:19%;
	height:30px;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
	margin:5px;
	border:1px solid #e5e5e5;
	line-height:30px;
	text-align:left;} /* 设置A标签样式 */
a:hover {color: red;background-color:#e5e5e5;border:1px solid #233333;} /* 设置A标签鼠标放上去的样式 */
h3{width:1200px;height:50px;background-color:#e5e5e5;} /* 设置H3标签样式 */
dt{max-width:1200px;} /* 设置DT标签样式 */
.mdui-btn-block{background-color:#e5e5e5;} /* 设置H3背景颜色 */
img{height:15px;margin-right:10px;margin-left:10px;} /* 设置图标样式 */
</style>
```

![](https://raw.github.com/MoXiaoCC/BookmarksBeautify/master/img/6.png)

**第三步**
全局替换`<H3`为
`<H3 class="mdui-btn mdui-btn-block"`

![](https://raw.github.com/MoXiaoCC/BookmarksBeautify/master/img/4.png)

**第四步**
谷歌浏览器导出的全局替换`ICON="`为
`><img src="`

![](https://raw.github.com/MoXiaoCC/BookmarksBeautify/master/img/5.png)

IE浏览器导出的书签全局替换`ICON_URI="`为
`><img src="`
