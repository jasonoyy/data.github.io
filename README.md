# jasonoyy.github.io

http://119.45.185.117/


<center>
  <font size="+2">常见问答：系统运行中可能会出现的问题 </font>
</center>
<hr>
</div>
<hr>
<p><font color=green>Q1</font>:程序怎样取得输入、进行输出?<br>
  <font color=red>A</font>:你的程序应该从标准输入Scanner cin = new Scanner(System.in);
  <br>
  并将结果输出到标准输出 
  <font color=blue>System.out.println();</font>: 

  推荐使用Java，系统也支持C++和Python等其它语言:<br>
  <br>下面代码是1000题的解答
  <br>
<pre><font color="blue">
import java.util.*;
public class Main{
	public static void main(String args[]){
		Scanner cin = new Scanner(System.in);
		int a, b;
		while (cin.hasNext()){
			a = cin.nextInt(); b = cin.nextInt();
			System.out.println(a + b);
		}
	}
}</font></pre>

<p><font color=green>Q2</font>:系统运行缓慢?<br>
  <font color=red>A</font>:
  <h4>请先在编程环境调试通过，运行成功再提交代码，每位同学每题可提交10次，<font color=red>多于10次提交者，该题期末成绩将会扣分</font>。
</h4>
  <br>

  <p><font color=green>Q3</font>:编译问题?<br>
  <font color=red>A</font>:1。请先选择正确你所使用的编程语言
  <br>
2.保证程序主类为Main，注意大小写
<br>

<p><font color=green>Q4</font>:自己定义的类该放哪?<br>
  <font color=red>A</font>:1。一定要放在Main类中
  <br>
  2.自定义的类注意一定要静态定义
  <br>
 
  <br>
具体如下：  
  <pre><font color="blue">
import java.util.*;
public class Main{
  public static class Node{// 注意一定要静态
		public String ID;
		public String name;
		public Node next;

		 Node(){
			this.ID="";
			this.next=null;
    }
  }
	public static void main(String args[]){
		Scanner cin = new Scanner(System.in);
  Node nd= new Node();
  ...  
  
  }
}</font></pre>
