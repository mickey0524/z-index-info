# z-index-info
有关z-index 的一些理解（包括static / relative / absolute / fixed）
首先，static是默认状态，是不受top，left等和z-index的影响的，这种时候使用margin的负px移动div，会将下方
的东西直接覆盖在当前div上
如果是使用relative等，则会先定位，然后再画图，就会使当前的div在下方div的上面

父亲和孩子拥有相同z-index的时候，孩子会覆盖父亲

兄弟拥有相同z-index的时候，后面的会覆盖前面的
