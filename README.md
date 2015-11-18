# MonthPicker
基于jQuery的月份选择器，提供web应用系统中常用的月份选择操作功能。
# 文件列表 #
+ monthPicker.js  组件选择器的主js
+ monthPicker.css 组件所依赖的样式
+ jquery.min.js   jQuery1.7.2类库
+ images           组件所依赖的图片

# 使用说明 #
### 调用示例 ###
<pre>
	<code>
		monthPicker.create('month_picker', {
		    trigger : 'month_trigger',
		    autoCommit : true,
		    defaultMonth : '201511',
		    callback : function(obj){
		        //设置回调句柄,obj是当前已经选择的时间对象
		    }
		});
	</code>
</pre>


### 参数说明 ###
##### id #####
组件月份选择回显的DOM元素ID
#####trigger#####
如果有额外的呼出结构，比如sample.html中的右侧向下的箭头，可以额外指定呼出选择面板的触发器
#####autoCommit#####
日期选择完毕后立即出发绑定的回调事件
#####returnDate#####
选择后回调传入的值是月份还是具体日期，默认是月份，如果需要日期，则设置为true
#####defaultMonth#####
初始化月份选择器时候指定的默认日期，形如：‘201510’
#####all_month_valid#####
是否所有月份都可选择，默认是false，则本月之后的月份不可选择，如果设置为true，则全部可选
#####callback#####
选择成功后提交调用的回调函数，传入已选择的格式化后的月份或者日期，如：‘2015-10’
