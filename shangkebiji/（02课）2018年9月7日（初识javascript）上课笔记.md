# 2018年9月7日（初识javascript）上课笔记

1.script标签写在哪？

	script标签只能放在head和body中底部

2.一个页面可以有多个script标签

3.注释：

	a. / ** /多行注释 
	
	b.  //单行注释

4.如果一个script标签已经用来去引入外部的Js文件了，那么再在里面代码没有意义的不要再在这种script里面写任何东西

5.type和language要么不写，要写一定得写对，推荐不写

6.可以直接在标签里面给当前标签添加事件，但是没有特殊的要求，我们不推荐在行内去写JS代码

	//<div id="wrap" onclick="alert(123);">wrap</div>
	
	//<a herf="javascript:alert("a标签被点击了！)">g</a>
	
	//<a herf="javascript:void(0)"></a>

7.注意事项：

	a.严格区分大小写
	
	b.功能字符都是半角字符
	
	c.语句结束 ；号（当然也可以选择不写分号）
	
	d.注意代码的缩进

8.弹窗与调试

	弹窗：alert("123")（直接展示内容）
	
	调试：console.log("234")

9.系统弹窗(需要接收)

	confirm("123456")确认值（判断确认或取消）
	
	prompt("123456")输入框（需要接收）

10.响应用户操作示例

	元素    节点   标签
	
	首先页面加载的时候就给我们需求的节点绑定一个事件反馈机制
	
		document.getElementById("id").onclick=function(){
	
			alert("快点击我呀！")
	
		}

11.操作HTML元素添加内容

	"=" 赋值的意思
	
		document.getElementById("id").innerHTML="123"





