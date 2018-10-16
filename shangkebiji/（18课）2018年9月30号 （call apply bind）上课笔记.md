2018年9月30号 （call apply bind）上课笔记

1.this在普通模式下指向顶层对象

   在严格模式下是underfind

2.函数可以借助于call来执行

```js
<script>
    function a(x,y){
    	console.log(x)
    	console.log(y)
    	console.log(this)
	} 
	//this指向的替代方式
	a(8,9)
	a.call(document,8,9)//call可以有n个参数，要错位指向
	a.apply(document,[8,9])//apply只能有两个参数
</script>
```

3.bind改变this的指向方式

```js
<script>
   function a(x,y){
    	console.log(x)
    	console.log(y)
    	console.log(this)
	} 
	function b(x){
    	x(7,5)	
	}
	b(a.bind(document))
	//或者：b.bind(10)()
	a.bind(document)//作用是被动执行  这样直接写是没音什么效果的
</script>
```

```js
<script>
    document.onclick=function(x,y){
    	console.log(x)
    	console.log(y)
    	console.log(this)
	}.bind({name:'阿飞'},5,4)//和call一样传参数，bind的作用，产生新的函数
</script>
```

4.新的API，低版本浏览器不支持 网址：https://caniuse.com/

```js

```

