*js 函数的参数声明中用 var 与不用 var的区别
	*var 声明的变量,作用域是当前 function 
	*没有声明的变量,直接赋值的话, 会自动创建变量,但作用域是全局的. 
	//----------------- 
	function foo() { 
		a = "aaaa"; 
	} 
	foo(); //  foo执行之后 
	alert(a); // 可以看到 "aaa" 
	//----------------- 
	如果用了 var 
	//----------------- 
	function foo() { 
		var a = "AAA"; 
	} 
	foo(); // 执行一次 foo 
	alert(a); // 出错!!! 变量未定义, 因为 foo 中声明的变量作用域只是 foo 函数. 