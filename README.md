# flex-demo
用felx布局搭建网页及相应式
## flex属性 解释在 index.html中

```
            /*
                决定主轴的方向  row | row-reverse | column | column-reverse
                row →;  row-reverse ←;column ↓ ；column-reverse ↑
            */
            flex-direction:row;
            /*
                flex-wrap属性定义，如果一条轴线排不下，如何换行。
                    nowrap 不换行
                    wrap 向下换行
                    wrap-reverse 向上换行
             */
            flex-wrap:wrap;
            /*flex-flow: <flex-direction> || <flex-wrap>;*/


            /*
                justify-content属性定义了项目在主轴上的对齐方式。
                    flex-start（默认值）：main-start对其
                    flex-end：main-end对其
                    center： 居中
                    space-between：两端对齐，项目之间的间隔都相等。
                    space-around：每个项目两侧的间隔相等。所以，项目之间的间隔比项目与边框的间隔大一倍。
             */
            justify-content:space-between;
            /*
                align-items属性定义项目在交叉轴上如何对齐。
                    flex-start：交叉轴的起点对齐。
                    flex-end：交叉轴的终点对齐。
                    center：交叉轴的中点对齐。
                    baseline: 项目的第一行文字的基线对齐。
                    stretch（默认值）：如果项目未设置高度或设为auto，将占满整个容器的高度。
             */
            align-items:stretch;
            /*
                align-content属性定义了多根轴线的对齐方式。如果项目只有一根轴线，该属性不起作用。
                    flex-start：与交叉轴的起点对齐。
                    flex-end：与交叉轴的终点对齐。
                    center：与交叉轴的中点对齐。
                    space-between：与交叉轴两端对齐，轴线之间的间隔平均分布。
                    space-around：每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍。
                    stretch（默认值）：轴线占满整个交叉轴。
             */
            align-content: flex-start ;

        
        [class*='child']{

            order: 0;/*order属性定义项目的排列顺序。数值越小，排列越靠前，默认为0。*/
            flex-grow: 1;/*flex-grow属性定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。*/
            flex-shrink: 1; /* flex-grow属性定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。 */
            /*
            flex-basis属性定义了在分配多余空间之前，项目占据的主轴空间（main size）。
            浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。
            */
            /*flex-basis: auto;*/

            /*flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]*/ /*简写*/
```

## flex搭建的 布局在 mypractice.html 中
其中 布局模板我进行了响应式
