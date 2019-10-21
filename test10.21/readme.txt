10.21日测验
在本地创建一个文件夹叫test10.21 ,文件夹中应含有5个html文件,分别命名为1.html等.再创建一个readme.txt文件,将这几个问题贴如其中,最后将html中的js代码贴到答的下方.

1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:         var h1 = document.getElementById('h1')
			var str1 = '你好'
			var str2 = '欢迎光临'
			h1.innerHTML = str1.concat(str2)

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:         var in1 = document.getElementById('in1')
			var btn = document.getElementById('btn')
			var h2 = document.getElementById('h2')
			btn.onclick=function(){
				h2.innerHTML = '存款金额为'+in1.value.padEnd(6,"0")
			}

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:         var h3 = document.getElementById('h3')
			var sun = 79387.348
			h3.innerHTML = sun.toFixed(2)

4.一张图片是一个相对路径img/head/,icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:   

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h5的元素中
答:         var h5 = document.getElementById('h5')
			var inp = document.getElementById('inp')
			var inpv = inp.value
			var but = document.getElementById('but')
			var h1 = document.getElementById('h1')
			but.onclick  = function(){
				if (inpv.toLowerCase = h1 ){
					h5.innerHTML = '验证正确'
				}else if(inpv.toUpperCase()= h1 ){
					h5.innerHTML = '验证正确'
				}else{
					h5.innerHTML = '验证错误'
				}
			}