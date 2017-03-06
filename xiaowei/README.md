###项目说明
---

本项目为`ife` 项目
##1. task3[踩过的坑]
###1)浮动，
    位置：中间放最后，左右栏的位置随意
        浮动会脱离当前所在的文档流，根据前面元素的位置决定浮动的位置。
        它的浮动的上面位置是和它前一个原来在标准流中的元素底部对应，而不是包裹它的外面的元素。
###2）定位，
    位置：没有要求
        子没办法撑起父级，高度塌陷。min-height
        [一般我们不使用position来对页面内部的元素进行具体的布局，这样容易导致问题且扩展性低]
###3)margin
    位置:中间在前面即可
    原理:所有元素都浮动,改变浮动位置
    坑:中间的min-width和左中右合起来的min-width
###4)flex布局
    http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html
``

##2.task4
###1)https://css-tricks.com/centering-css-complete-guide/
    水平:inline---text-align:center

         block---width:xx px;
                 margin:0 auto;
         a)more than one block---外包裹块text-align:center;
                               里块display:inline-block;max-width:xx px;
         b)more than one block---外包裹块display:flex;justify-content:center;max-width:xx px;
    垂直:a)inline---padding-top:30px;padding-bottom:30px;
        b)inline---height:100px;line-height:100px;


        a)multiple lines---外包裹块display:table;
                           里块display:table-cell;vertical-align:middle;
        b)multiple lines---table>tr>td
        c)multiple lines---display: flex;flex-direction: column;justify-content: center;
        d)multiple lines---ghost element[ghost element.html]


        a)block---[04_position.html]
        b)block---[04_transform.html]