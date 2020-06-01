1. 圣杯布局和双飞翼布局的理解和区别，并用代码实现？ 
两者是为了解决三栏布局中间主要内容优先加载的问题（两侧浮动，中间宽度自适应）      
双飞翼布局不仅能满足main处于优先加载的地位，而且更好的解决圣杯布局的错乱问题，css更简单，缺点是增加了一个无意义标签    
https://www.jianshu.com/p/137c1037c991       
    
2.CSS3有哪些新增的特性?   
边框圆角    
border-radius     
盒子阴影    
box-shadow  
文字阴影  
text-shadow  
2d,3d 变换  
transform  
过度动画  
transition  
自定义动画化animation  
rgba透明度  
在rgb上设置了透明度  

3.在页面上隐藏元素的方法有哪些？       
占位:    
visibility:hidden    
margin-left:-100%    
opacity:0    
transform:scale(0)    
不占位:     
display:none     
width:0; height:0; overflow:hidden;    
仅对块内文本元素:    
text-indent: -9999px    
font-size:0  

2020/5/27<br>
1. 介绍⼀一下标准的css的盒⼦模型?与IE的盒⼦模型有什什么不不同?<br>
CSS盒⼦子模型: 外边距(margin) 内边距(padding) 边框(border) 内容区(width、height) CSS盒⼦模型与低版本IE的盒⼦模型的区别主要在于:宽和⾼不一样 标准的CSS的盒⼦模型的宽高:内容区的宽高 低版本IE的盒⼦子模型的宽高:内容区+内边距+边框<br><br>
2. display有哪些值?说明他们的作⽤用。position的值relative和absolute定位原点是? block 像块级元素⼀一样显示，元素前后会带有换行符。
none 此元素不不会被显示。<br>
inline-block ⾏内块元素<br>。
list-item 此元素会作为列表显示。<br>
inline 此元素会被显示为内联元素，元素前后没有换⾏行行符。 table 此元素作为块级表格来显示<br>
position:relative<br>
相对于⾃身文档流的位置进行偏移，不不会使得元素脱离⽂档流，不不影响元素本身特性<br>
position:absolute<br>
相对于最近⼀一个有定位的⽗元素偏移，使元素完全脱离⽂档流<br>
position:fixed<br>
⽣生成固定定位的元素，相当于浏览器窗口进行定位，脱离⽂档流<br>
position:static<br>
默认值，元素出现在正常的流中<br>
##absolute与fixed共同点与不不同点<br> 
A、共同点: <br>
1.改变⾏内元素的呈现⽅方式,display被置为block;<br> 
2.让元素脱离普通流,不占据空间; 3.默认会覆盖到⾮定位元素上;<br>
B、不不同点: <br>
absolute的”根元素“是可以设置的,而fixed的”根元素“固定为浏览器窗⼝。 当你滚动⽹页,fixed元素与浏览器窗口之间的距离是不变的。<br><br>
3. 为什什么要初始化css样式?<br>
CSS初始化是指重设浏览器的样式。不同的浏览器默认的样式可能不尽相同，所以开发时的第⼀一件 事可能就是如何把它们统⼀一。如果没对CSS初始化往往会出现浏览器之间的⻚面差异。每次新开发 ⽹站或新网页时候通过初始化CSS样式的属性，为我们将⽤到的CSS或html标签更加⽅便准确，使得我们开发⽹页内容时更加⽅便简洁，同时减少CSS代码量量，节约⽹⻚下载时间。 当然，初始化样式会对SEO有⼀一定的影响，但⻥和熊掌不不可兼得，但力求影响最⼩的情况下初始化。 SEO:汉译为搜索引擎优化。是⼀种⽅式:利用搜索引擎的规则提⾼网站在有关搜索引擎内的自然排名<br><br>
4. CSS 选择符有哪些? 优先级算法如何计算? <br>
1.id选择器( # myid)<br>
2.类选择器(.myclassname)<br> 
3.标签选择器(div, h1, p)<br>
4.相邻选择器(h1 + p) <br>
5.⼦子选择器(ul > li)<br>
6.后代选择器(li a)<br>
7.通配符选择器( * )<br>
8.属性选择器(a[rel = "external"])<br> 
9.伪类选择器(a: hover, li: nth - child)<br>
!important>⾏内样式>ID选择器>类选择器>标签>通配符>继承>浏览器默认属性 同⼀级别中后写的会覆盖先写的样式。<br><br>
5. display:none 和visibility:hidden的区别?<br>
如果给一个元素设置了display: none，那么该元素以及它的所有后代元素都会隐藏，它是前端开发⼈员使⽤频率最高的⼀一种隐藏⽅方式。隐藏后的元素⽆法点击，⽆无法使⽤屏幕阅读器等辅助设备访 问，占据的空间消失。<br>
给元素设置visibility: hidden也可以隐藏这个元素，但是隐藏元素仍需占⽤与未隐藏时⼀一样的空间，也就是说虽然元素不可⻅了，但是仍然会影响⻚面布局。<br>
<br>
2020/6/1<br>
1. overflow有哪些属性？<br>
visible	默认值。内容不会被修剪，会呈现在元素框之外。<br>
hidden	内容会被修剪，并且其余内容是不可见的。<br>
scroll	内容会被修剪，但是浏览器会显示滚动条以便查看其余的内容。<br>
auto	如果内容被修剪，则浏览器会显示滚动条以便查看其余的内容。<br>
inherit	规定应该从父元素继承 overflow 属性的值。<br>

2. 什么叫做外边距折叠？<br>
块级元素的上下外边距(margin)在某些情况下会合并（折叠）起来，合并之后的大小为较大的margin。注意浮动和绝对定位的元素的margin从不折叠。<br>
1.（垂直方向上）相邻的两个元素<br>
2.父元素和第一个／最后一个子元素之间<br><br>

3.有哪项方式可以对一个DOM设置它的CSS样式？<br>
1.外部样式表，引入一个外部css文件<br>
2.内部样式表，将css代码放在 <head> 标签内部<br>
3.内联样式，将css样式直接定义在 HTML 元素内部<br><br>
    
4. 怎样用css绘制一个三角形？<br>
将一个div的宽度和高度，都设置为0，设置div四个边框的宽度，并利用transparent属性隐藏三个边框，只留下一个边框，就可得到一个三角形？如果是直角三角形，则隐藏2个相邻的边框，剩下2个相邻的边框就拼成了一个直角三角形。<br>
https://www.jianshu.com/p/9a463d50e441<br>


