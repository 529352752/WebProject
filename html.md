
1.页面导入样式时，使用link和@import有什么区别？  
link外部调用       
<link rel="stylesheet" rev="stylesheet" href="CSS文件" type="text/css" media="all" />      
@import外部调用(必须在<style></style>之间使用   
<style type="text/css" media="screen">          
@import url("CSS文件");    
</style>    
区别1:link是XHTML标签，除了加载CSS外，还可以定义RSS,定义rel连接属性等;@import属于CSS范畴，只能加载CSS      
（XHTML是一种标记语言，表现方式与HTML类似，不过语法上更加的严格   ） 
（rel属性规定当前文档与被链接文档之间的关系）。	   
区别2:link引用CSS时，在页面载入时同时加载；@import需要页面完全载入以后加载   
区别3:link是html元素，不存在兼容问题;@import是CSS2.1才又的语法，只可在IE5+才能识别       
区别4:通过js操作DOM,可以插入link标签来改变样式;由于DOM方法是基于文档的，无法使用@import方式插入样式        
    
2.html的元素有哪些(包含H5)?    
行内元素    
<span> <a> <br> <b>加粗 <strong>加粗 <img> <sup>上标 <sub>下标 <i>斜体 <em>斜体 <del>删除线 <u>下划线 <input> <textarea> <selec>   
块级元素   
<address> <h1-h6> <hr> <p> <pre> <blockquote>段落缩进 <ul> <ol> <dl> <table> <form> <div>     
块级元素的特点   
1. 高度，行高以及边距都可以控制。
2. 在新行上开始，占据一整行。
3. 可以容纳内联元素和其他块元素。

行内元素的特点
1. 行内元素只能容纳文本或者其他行内元素。
2. 和其他元素在一行上
3. 不可设置宽高，宽高随文本内容变化，可以设置行高line-height

H5新增元素
<article> <aside> <nav> <section> <header> <footer> <datalist>定义下拉 <fieldset>可将表单内的相关元素分组

