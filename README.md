iconfontdemo
============

##1.安装iconfont字体编辑工具FontLab
[http://pan.baidu.com/share/link?shareid=1561156774&uk=2416921138](http://pan.baidu.com/share/link?shareid=1561156774&uk=2416921138)

 

##2.FontLab使用步骤
* 新建一个字体文件(File->New)
* 双击任意一个字符，使其为可编辑状态
* 邮件点击该字符，依次点击copy,paste，在末尾会生成一个新的字符
* 双击该字符，即可为编辑字符状态，任意画一个图形后关闭
* 对该字符点击右键->Properties，修改Name和Unicode（如：A001），点击Apply
* 完成后，点击File->Generate Font，保存为iconfont.ttf，完成字体编辑


##3.使用在线工具生成eot、svg、woff格式以适应各浏览器
* [http://www.fontsquirrel.com/tools/webfont-generator](http://www.fontsquirrel.com/tools/webfont-generator)
* 点击Addfonts -> 选择刚保存的iconfont.ttf，选择BASIC，然后download,即可生成以上格式


##4.生成css
```css
  @font-face {font-family: 'iconfont';
    src: url('iconfont.eot'); /* IE9*/
    src: url('iconfont.eot?#iefix') format('embedded-opentype'), /* IE6-IE8 */
    url('iconfont.woff') format('woff'), /* chrome、firefox */
    url('iconfont.ttf') format('truetype'), /* chrome、firefox、opera、Safari, Android, iOS 4.2+*/
    url('iconfont.svg#iconfont') format('svg'); /* iOS 4.1- */
}

.iconfont{font-family:"iconfont"; font-style:normal;-webkit-font-smoothing: antialiased; -webkit-text-stroke-width: 0.2px; -moz-osx-font-smoothing: grayscale;}
```

##5.显示html
```html
  <i class="iconfont">&#xB001;</i>
```
