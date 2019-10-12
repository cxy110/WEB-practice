<1 类选择器>
   .+类名{}

<2 ID选择器>
   #+ID名{}

<3 元素选择器>
  元素名{}

<4 属性选择器> 
   1.[属性名]{}
   2.[属性名=具体的值]{} 比如: [href="http:www.baidu.com"]

   3. 其他选择器[属性名1][属性名2]{}
        如上就是为某个选择器下同时有属性1和属性2的html内容添加样式
   4.[属性名~=value]{}
        表示在属性中包含有独立的value
        比如:[title~=flower]  -->  <img src="/i/eg_tulip.jpg" title="tulip flower"/>   
   5.[属性名*=value]{}
        属性中只要能拆分出value就行
        比如:[title*=flower]   -->  <img src="/i/eg_tulip.jpg" title="ffffflowerrrrrr" />     
    6.[属性名^=value]{}
        属性中只要以value开头就可以

     7..[属性名$=value]{}
         属性只要以value结尾就行       
<5 伪类选择器>
  是加在选择器后面用来指定元素状态的关键词
       语法:  selector:pseudo-class{}
   :link
   :visited
   :hover
   :active
   伪类选择器前是一个冒号

<6 伪元素选择器 >
      语法: selector::pseudo-element{}
    如:
    before ,after等
    伪元素选择器前是两个冒号

    如果前面没有指定选择器就是对全体相应的有效

<7 关系选择器>
   1. 后代选择器 
      祖先元素 后代元素
   2子元素选择器
      父元素>直系子元素
   3.兄弟选择器
      大哥元素+小弟元素(大哥元素后面紧邻的小弟元素) 
   4.哥哥元素~弟弟元素(哥哥元素后面所以的弟弟元素)  