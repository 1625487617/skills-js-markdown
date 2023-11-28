# js #
## 基础 ##
### 输入输出 ###
			document.write
			console.log
			
			prompt(输入)
### 交互效果 ###
			页面弹出输入框
			计算圆的面积（内部处理）
			页面输出
###  字面量 ###
			number
			string
			boolean
			null
			undefined
### 运算符
			三元
				条件？满足条件执行表达式：不满足条件执行表达式
### 数组的增删改查
			增
				arr.push(元素1，元素2，，，，)
					还可以返回新数组的长度
					从数组后面加
				arr.unshift(元素1，元素2，，，，)
					加数组前面
			删
				arr.pop（）
					删除最后一个
				arr.shift()
					删除第一个
				arr.splice(start,deleteCount){如果不写deleteCountn那就删完}
### 函数
			function关键字
			匿名函数
				let fn=function(x,y)
				先声明表达式再调用
				立即执行函数
					（function（形参）{函数内容}）（实际参数）
					（function（）{}（））
					不用再调用
				子主题 4
		转换为booleanl类型
			false
				0,null,undefined,nan
			true
				其余
### 对象
			let 对象名 {属性：（变量）}
			增删改查
				删：delete
				查
					对象名.属性名
					对象名[‘属性名’]
			遍历对象
		内置函数
			math
## APIs
### DOM-获取元素（操作网页内容）
			DOM对象
				html的标签->js里面的对象
			document对象
				DOM自带对象：用来访问和操作页面
			获取DOM元素
				语法：document.querySelector('')
				id:语法：document.querySelector('#')
				语法：document.querySelector('ul li :first - child')
				总结：和css很相似
					子主题 1
				参数
					‘css选择器’
				返回值
					css匹配的第一个元素，一个html对象
				获取多个
					语法：document.querySelectorALL('')
					不能直接修改
					子主题 3
### 操纵元素内容
				innertext
					获取文本不解析，不识别标签
				innerHTML
					能识别标签
			操作元素属性
				常用
					子主题 1
				样式
					style(box.style.width)
					类
						先定义一个box的css然后div.className = 'box',直接把整个类的属性放过来，div.className = 'nav box'这种情况表明两种情况的CSs都需要（直接使用会覆盖以前的类名）
					classlist（最常用）(不用担心覆盖)
						add
							子主题 1
						remove
						toggle
				表单元素
					表单可以用value来获得表单里面的值，但是button不一样，需要用innerhtml
					例如：disabled checked selected
					子主题 3
				自定义  
					data开头
					dataset（获取关键字）
			定时器-间歇函数
				setinterval( 函数 ，间隔时间（毫秒）)
				定时器会返回自己独一无二的序号
				关定时器
					获取：let n =setinterval(....)
					关闭：clearinterval()
	分支主题 3
	分支主题 4
