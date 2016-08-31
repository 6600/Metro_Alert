

###notie.alert

|      属性     |     含义      |      初始值     |    重要性      |
| ------------- |:-------------:| ------------- |:-------------:|
| 参数1     |提示的类型 |  1.提示 2.警告 3.错误    |必须 | 
| 参数2     |提示的内容 |  无     |必须 | 
| 参数3     |自动消失时间 |  2s     |必须 | 



##代码展示
```javascript
<script>
    function success() {
		notie.alert(1, 'Success!', 2);
	}

	function warning() {
		notie.alert(2, 'Warning<br><b>with</b><br><i>HTML</i><br><u>included.</u>', 2);
	}

	function error() {
		notie.alert(3, 'Error.', 2);
	}

	function info() {
		notie.alert(4, 'Information.', 2);
	}

	function confirm() {
		notie.confirm('Are you sure you want to do that?<br><b>That\'s a bold move...</b>', 'Yes', 'Cancel', function() {
			notie.alert(1, 'Good choice!', 2);
		});
	}

	function input() {
		notie.input('Please enter your email address:', 'Submit', 'Cancel', 'email', 'name@example.com', function(value_entered) {
			notie.alert(1, 'You entered: ' + value_entered, 2);
		});
	}

</script>

<script src="notie.js"></script>
</body>
```
##效果演示：
![mahua](http://myweb-10017157.file.myqcloud.com/png/131171314301850475.png)
