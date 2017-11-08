

## index.html

层叠元素的显示的顺序，可以参考[这里][stacking-of-float]: 

1. root元素的背景和边框;
2. 按顺序显示非定位block子元素;
3. 浮动元素;
4. 按顺序显示非定位inline子元素;
5. 按顺序显示定位元素;

*ps: 在该实例中，给float元素增加z-index:999，没有效果，因为z-index对position:static的元素没效果*<br/>
*所以给float元素增加position:relative后就有效果了*


设置了z-index的元素会单独形成stack context, 下面看看三个例子:

:pencil2: [example1](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/Stacking_context_example_1)<br/>
:rotating_light: [example2](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/Stacking_context_example_2)<br/>
:penguin: [example3](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/Stacking_context_example_3)<br/>

## reference

1. [Understanding CSS z-index](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index) <br/>
2. [z-index对非定位元素不起作用](https://stackoverflow.com/questions/579753/css-floating-w-overlap) <br/>

[stacking-of-float]: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/Stacking_and_float "float的z-index" 
