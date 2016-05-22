# HaoAmap
Auto show the address with amap.

#HaoAmap使用方法：#
1. 在html里引入jquery.js webapi.amap.com/maps haoamap.js 三个js文件。
2. 使用以下方案，将地址数据放置在对应的input中即可。
	1. 如果地址所在input的class为input_which_is_address，则haoamap.js会在页面载入后自动渲染图片。
	2. 如果地址所在input不含默认class,则需要在页面载入或数据更新后，自行调用HaoAmap.init(inputNode)的方法来进行地图渲染。（inputNode为dom元素，如$('input')[0]）
3. 如果在地图渲染完成后，通过js更改了地址所在input的值，可以使用$(inputNode).trigger('change')的方法，来手动触发更新。
