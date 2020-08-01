# jasonoyy.github.io

http://119.45.185.117/
#Q1:程序怎样取得输入、进行输出?
A:你的程序应该从标准输入Scanner cin = new Scanner(System.in);
并将结果输出到标准输出 System.out.println();: 推荐使用Java，系统也支持C++和Python等其它语言:

下面代码是1000题的解答

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
}
#Q2:系统运行缓慢?
A:

请先在编程环境调试通过，运行成功再提交代码，每位同学每题可提交10次，多于10次提交者，该题期末成绩将会扣分。

#Q3:编译问题?
A:1。请先选择正确你所使用的编程语言
2.保证程序主类为Main，注意大小写
#Q4:自己定义的类该放哪?
A:1。一定要放在Main类中
2.自定义的类注意一定要静态定义

具体如下：


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
}
