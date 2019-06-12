经典案例练习
<p>设置y=5, 计算出 x=++y,并显示结果。</p>
    <button onclick="myFunction()">press here</button>
    <p id="demo"></p>
    <script>
      function myFunction()
      {
          var y=5;
          var x=++y;
          var demoP=document.getElementById("demo")
          demoP.innerHTML="x=" + x + ",y=" + y;
      }
     </script>

<p>if else 的用法</p>
    <script>
        var d =new Date();
        var time = d.getHours();
        if(time<10)
        {
            document.write("<br>早上好</br>");
        }
        else if (time>=10 && time<16)
        {
            document.write("<br>下午好</br>");
        }
        else{
            document.write("<br>晚上好</br>")
        }
    </script>


    输出一个数字，满足条件如下
    <script>
        var a = parseInt(prompt ("请输入第一个数字"));
        if(a%5 == 0 && a % 6 == 0){
            alert ("这个数字同时能被5和6整除");
        }
        else if(a%5 == 0 &&a % 6 != 0)
        {
            alert("这个数字能同时被5整除,但是不能被6整除")
        }
        else if(a % 5 != 0 && a % 6 == 0){
            alert("这个数字能同时被6整除,但是不能被5整除")
        }
        else if (a % 5!= 0 && a % 6 != 0)
        {
            alert("这个数字既不能被5整除,也不能被6整除");
              
        }
    </script>

    1-1000中所有能被5整除，或者被6整除的数字，在控制台输出
    <script>
        for(var i = 1;i<=1000; i++){
            if(i%5 ==0 ||i%6 ==0){
                console.log(i);
            }
        }
    </script>

    如果报到能被7整除的数字，
    或者尾数是7的数字，就算踩地雷了，
    请在控制台输出1~60之间所有的“安全数”。
    比如1、2、3、4、5、6、8、9、10、11、12、13、15、16、18……
    <script>
        for(var i = 1;i<=60;i++){
            if(i%7 !=0 && i%10!=7)
            console.log(i);
        }
    </script>


    被1和自己整除，
    即：它的因数个数是2。
    比如2、3、5、11、13、17、19、23……用户输入一个数字，
    弹出这个数字是否是质数。
    <script>
        var number = parseInt(prompt("请输入一个数字"));
        var amount =0 ;
        for(var i = 1; i<=number; i++){
            if (number%i ==0){
                amount++;
            }
            if(amount =2){
                alert("这是质数");
            }
            else{
                alert("这不是质数");
            }
        }
    </script>

    斐波那契函数
    <script>
    function  fibonacci(n){
        if (n ==1 || n ==2){ 
        return 1
    }
    return fibonacci(n-1) + fibonacci(n-2)
}
    console.log(fibonacci(3));
    </script>