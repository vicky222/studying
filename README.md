# studying
<!DOCTYPE html>
<html>
 <head>
  <title> 事件</title>  
  <script type="text/javascript">
   function count(){
       
    var num01=document.getElementById("txt1").value;
    var num11=parseInt(num01);
    //获取第一个输入框的值
	var num02=document.getElementById("txt2").value;
	var num22=parseInt(num02);
	//获取第二个输入框的值
	var select=document.getElementById("select").value;
	//获取选择框的值
	var num;
	switch(select){
	    case "+":num=num11+num22; break;
	    case "-":num=num11-num22; break;
	    case "*":num=num11*num22; break;
	    case "/":num=num11/num22; break;
	}
	//通过下拉框来选择的值来改变加减乘除的运算法则
    document.getElementById("fruit").value=num;//设置结果输入框的值 
    
   }
  </script> 
 </head> 
 <body>
   <input type='text' id='txt1' /> 
   <select id='select'>
		<option value='+'>+</option>
		<option value="-">-</option>
		<option value="*">*</option>
		<option value="/">/</option>
   </select>
   <input type='text' id='txt2' /> 
   <input type='button' value=' = ' onclick="count()"/> <!--通过 = 按钮来调用创建的函数，得到结果--> 
   <input type='text' id='fruit' />   
 </body>
</html>
