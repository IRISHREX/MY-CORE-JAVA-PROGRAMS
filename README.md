# MY-CORE-JAVA-PROGRAMS
my core java a-z programs are stored for learning purpose.
MY FIRST PROGRAM:
package first;

public class ClassA
{ 
	int a=10;
	int b= 20;
	void meth1()
	{
	ClassA obj=new ClassA();
	obj.meth3();
			System.out.println("meth 1 called");
			System.out.println(a+b);
			
	}
	void meth2()
	{
		System.out.println("meth 2 called");
		System.out.println(a-b);
	}
	void meth3()
	{
		System.out.println("meth 3 called");
		System.out.println(a*b);
		ClassA obj=new ClassA();
		obj.meth2();
		}
	void meth4()
	{
		System.out.println("meth 4 called");
        System.out.println(a/b);
		ClassA obj=new ClassA();
		obj.meth1();
	}
	void meth5()
	{
		System.out.println("meth 5 called");
		System.out.println(a%b);
		ClassA obj=new ClassA();
		obj.meth6();
		
	}
	void meth6()
	{
		System.out.println("meth6 called");
		ClassA obj=new ClassA();
		obj.meth4();
		System.out.println("done ");
	}
	public static void main (String []args)
	{
		ClassA obj=new ClassA();
		obj.meth5();
}
}


PROGRAM 2:
package first;

public class ClassB
{
	void meth1()
	{
		System.out.println(10);
		System.out.println(20);
		System.out.println("end");
		
	}
int meth2 (int a, int b, int c)
{
	System.out.println(a);
	ClassB bobj=new ClassB();
	String s= bobj.meth5(100,"java is Manasa");
	System.out.println(s);
	return a-b-c;
	
}
String meth3 (String s,int b, int d )
{
	System.out.println (b+d);
	return s;
}
int meth4 (int c, int k)
{
	System.out.println(k);
	ClassB bobj=new ClassB();
	int result=bobj.meth2(50, 50, 50);
	System.out.println(result);
	return k+10;
}
String meth5(int a, String l)
{
	System.out.println(a+a);
	ClassB aobj=new ClassB();
	String s=aobj.meth3("hi",15,10);
	System.out.println(s);
	return l;
}
public static void main (String[]args)
{
	ClassB bobj=new ClassB();
	System.out.println("start");
	int result=bobj.meth4(20,10);
	System.out.println(result);
	bobj.meth1();

}
}
PROGRAM 3:
package first;

public class ClassC 
{
	float methx(int a,int b,int c)
	{
		System.out.println( a+b);
		System.out.println( (b+a)/(c-b) );
		return a+b+300;
	}
	String meth2 (int a, int b,int c)
	{
		System.out.println("sum is "+ (a+b));
		return "WAYYYY";
	}
	public static void main(String[]args)
	{
		ClassC aobj=new ClassC();
		double x=aobj.methx(1000, 200, 400);
		System.out.println("what is going on"+x);
		String y=aobj.meth2(10, 10, 10);
		System.out.println("what is goibg on 2....."+ y );
}
}

PROGRAM 4:
package first;

public class ClassD {
	void display()
	{
		System.out.println("callingC ....");
		
	}
public static void main(String[]args)
{
	ClassD obj=new ClassD();
			obj.display();
			ClassA aobj=new ClassA();
			aobj.meth1();
			aobj.meth2();
	ClassC bobj=new ClassC();
	bobj.methx(1000, 110, 110);
	ClassB cobj=new ClassB();
	cobj.meth4(200,100);
	
}
}

PROGRAM 5:
package first;

public class ClassE {
	void display()
	{
		System.out.println("callingC ....");
		
	}
public static void main(String[]args)
{
	ClassE obj1= new ClassE();
	ClassA obj2= new ClassA();
	ClassD obj3= new ClassD();
	int val1=obj1.hashCode();
	int val2=obj2.hashCode();
	int val4=obj3.hashCode();
	System.out.println("hash code of obj1...." +val1 );
	System.out.println("hash code of obj1...." +val4 );
	System.out.println("hash code of obj2...." +val2 );
	float c=(val1+val2)/val1;
	float s=val4;
	System.out.println(s);
	System.out.println(c);
	boolean result1= obj1.equals (obj2);
	boolean result2= obj2.equals (obj2);
	boolean result3= obj1.equals (obj3);
	System.out.println("case 1====>" +result1);
	System.out.println("case 2====>" +result2);
	System.out.println("case 3====>" +result3);


}
}

PROGRAM 6:
package med;

public class ClassF 
{
	void meth1()
	{
		System.out.println(10);
		System.out.println(20);
		System.out.println(30);
		System.out.println(40);
		ClassF aobj=new ClassF();
		System.out.println( aobj.meth2());
		return;
		
	}
	int meth2()
	{
	
int a=25;
if ((a+a)>=50)
		{
			System.out.println("alive");
		return 100;
	}
		else
		{
			System.out.println("dead");
			return 200;	
		}


    
	}
	
		
	

public static void main(String[]args)
{
	ClassF aobj=new ClassF();
	aobj.meth2();
	aobj.meth1();
}
}

PROGRAM 7:
 
package med;

public class ClassG
{
void meth1()
{
	System.out.println("method1 ....");
	int a=100;
	int b=200;
	int c=a+b;
	System.out.println("lets sum up" + c);
}
int meth2(int a,int b,int c)
{
	System.out.println("method2 ....");
	System.out.println("lets see what happened..." + (a+b));
	System.out.println("lets see what happened..." + c);
	return 10000;
}
int display(	int d)
{
	System.out.println("Display method........");
	ClassG aobj=new ClassG();
	int val1=aobj.hashCode();
	System.out.println("lets experint everything.."+ val1  );
	return d;
}
int show(int x,int y)  
{
	System.out.println("show method....."+ (x+y));
	return 10;
	
}

	public static void main(String[] args) {
		System.out.println("main method....");
		ClassG aobj=new ClassG();
		aobj.meth1();
		int c=aobj.meth2(10,100,0);
		int d=aobj.display(993255719);
    System.out.println("METH 2 C IS...." +c);
    System.out.println("DISPLAYS D IS" +d);
    System.out.println("FIRST METHOD DATA THEN MAIN PRINT DATA" + (aobj.show(10,10)));
	System.out.println("END ....");
    
	}

}
PROGRAM 8:
package med;

public class ClassH {
	static int b=100;
	int c=101;
	int a=999;

	void meth1 ()
	{
		System.out.println("meth1 called.......");
		int a=11;
	int b= 12;
		System.out.println("test to print  local variable.............." + a +b );
		System.out.println("test to print instance  variable.............." +c);
		System.out.println("test to print static variable.............." +ClassH.b);
	}
	void meth2 ()
	{
		System.out.println("meth2 called.......");
		System.out.println("test to print instance  variable.............." +c);
		System.out.println("test to print static variable.............." +ClassH.b);
		System.out.println("test to print static variable from instance veriable .............." +new ClassH().a);
new ClassH().meth3();
	
	}


	void meth3 ()
	{
		System.out.println("meth3 called.......");
		System.out.println("test to print  local variable without  using class.............." + a +b );
		System.out.println("test to print static variable.............." +new ClassH().c);
	}

	public static void main(String[] args)
	{
	ClassH aobj=new ClassH();
	aobj.meth1();
	aobj.meth2();

	}

}
PROGRAM 9:
package med;

public class ClassI {

	 ClassI()
	{
		System.out.println("non parametrilized constructor called");
		
	}
	ClassI(int a)
	{

		System.out.println("parametrilized constructor called"  + a);
		new ClassI().display();

	}
	void display()
	{
		System.out.println(" display method called 1");
	}

	public static void main(String[] args) 
	{
		System.out.println(" main method called 1");
		new ClassI( 10).display();

	

	}

}

PROGRAM 10:
package project2;

public class ClassJ {
	ClassJ()
	{
		System.out.println(10);
		new ClassJ(40).show(50);
		System.out.println(70);
		
	}
	void show(int a)
	{
		System.out.println(a);
		System.out.println(60);
	
	}
	ClassJ (int a)
	{
		System.out.println(20);	
		System.out.println(30);
		System.out.println(a);
	}
	void display() 
	{
		System.out.println(80);
		System.out.println(90);
	}

	public static void main(String[] args)
	{
ClassJ aobj=new ClassJ();
aobj.display();


	}

}

PROGRAM 11:
package project2;

public class ClassK {
	public ClassK()
	{
		System.out.println("sunday");
		ClassK aobj=new ClassK(10);
		System.out.println("tuesday");
		String s= aobj.display("chalange accepted");
		System.out.println(s);
	}
	 protected ClassK(int temp)
	{
		System.out.println("saturday");
	new ClassK(10,20);
		System.out.println("monday");
	}
	 String display(String s)
	{
		System.out.println("in the next statement im returning String value");
		return s;
	}
	 ClassK (int data,int temp)
	 {
			System.out.println("thursday");
		
	 }

	public static void main(String[] args) 
	{
		ClassK obj=new ClassK();
		String l=obj.display("meow");
		System.out.println( "out put varified" +l); 
PROGRAM 12:
package project2;

public class ClassL
{ 
	final int a=10;
	static int b =111;
	final static int c=999;
	static int l=new ClassL().show();
	
int show()
{
	System.out.println("--STATIC MRTHOD AND BLOCK--");
	System.out.println("=======================");
		System.out.println("***SHOW METHOD***");
		System.out.println("=======================");
		System.out.println("instance variable"+new ClassL().a);
		System.out.println("static variable"+b);
		System.out.println("=======================");
		return 100;
}
	static
	{
		System.out.println("***STATIC METHOD 1***");
		System.out.println("=======================");
		System.out.println("instance variable"+new ClassL().a);
		System.out.println("static variable"+b);
		System.out.println("=======================");
	}

	public static void main(String[] args)
	{
		System.out.println("***main METHOD***");
		System.out.println("=======================");
  }
	static
	{
		System.out.println("***STATIC METHOD  2**");
		System.out.println("=======================");
		System.out.println("instance variable"+new ClassL().a);
		System.out.println("static variable"+c);
		System.out.println("=======================");
	}

	}
PROGRAM 13:
package project2;

public class ClassM 
{
	void display()
	{
		int a=10;
		a++;
		++a;
		System.out.println("**__INCRIMENT AND DECRIMENT__**");
		System.out.println(a++);
		System.out.println(a);
		System.out.println(--a);
		System.out.println(++a);
		--a;
		a--;
		System.out.println(a++);
		System.out.println(--a);
		a++;
		System.out.println(++a);
		System.out.println(a);
		a--;
		a++;
		System.out.println(++a);
		System.out.println(a);
	}

	public static void main(String[] args) 
	{
		ClassM aobj=new ClassM();
		aobj.display();

	}

}

PROGRAM 14:
package project2;

public class ClassN {

	public static void main(String[] args) 
	{
	int a=10;
	int b=20;
	int c;
	int d;
	c=++b;
	d=a-- ;
	c++;
System.out.println("**___INCRIMENT AND DECREMENT___**");
	System.out.println("a===>" +a);
	System.out.println("b===>" +b);
	System.out.println("c===>" +c);
	System.out.println("d===>" +d);


	}

}

PROGRAM 15:
package project2;

public class ClassO {
	int display()
	{
		System.out.println("============================");
		System.out.println("***IMPLICIT TYPE CASTING***");
		System.out.println("============================");
		byte b=10;
		int i=b;
		System.out.println("byte value===>" +b);
		System.out.println("int value===>" +i);
		char c='A';
		int x=c;
		System.out.println("char value===>" +c);
		System.out.println("int value===>" +x);
		System.out.println("============================");
		return x;
		
	}
	void show()
	{
		System.out.println("***EXPLICIT TYPE CASTING***");
		System.out.println("============================");
		int i=500;
		byte b=(byte)i;
		System.out.println("int value===>" +i);
		System.out.println("byte value===>" +b);
		float f1=10.999f;
		byte b2=(byte)f1;
		System.out.println("float value===>" +f1);
		System.out.println("byte value===>" +b2);
		System.out.println("============================");
	}

	public static void main(String[] args) 
	{
		new ClassO().display();
		new ClassO().show();

	}

}

PROGRAM 16:
package project2;

public class ClassP 
{
void meth1() {
	System.out.println("***METH1***");
	int a=10;
	if (a<10)
	{
		System.out.println("hi");
		System.out.println("condition is true===>");
	}
	System.out.println("hello");
	System.out.println("condition is false===>");
	ClassP aobj=new ClassP();
	aobj.meth2();
}
void meth2()
{
	System.out.println("***METH2***");
	int a=10;
	if (a<20)
	{
		System.out.println("if  block executed");
		System.out.println("condition is true");
		ClassP aobj=new ClassP();
		aobj.meth4();
	}
	else
	{
		System.out.println("else  block executed");
		System.out.println("condition is false");
		ClassP aobj=new ClassP();
		aobj.meth3();
	}
}
	void meth3()
	{
		System.out.println("***METH3 is called coz its false***");
	}
	void meth4()
	{
		System.out.println("***METH4 called coz its true***");
}
public static void main(String[]args)
{
	ClassP aobj=new ClassP();
	aobj.meth1();
}
}

PROGRAM 17:
package project2;

public class ClassL
{ 
	final int a=10;
	static int b =111;
	final static int c=999;
	static int l=new ClassL().show();
	
int show()
{
	System.out.println("--STATIC MRTHOD AND BLOCK--");
	System.out.println("=======================");
		System.out.println("***SHOW METHOD***");
		System.out.println("=======================");
		System.out.println("instance variable"+new ClassL().a);
		System.out.println("static variable"+b);
		System.out.println("=======================");
		return 100;
}
	static
	{
		System.out.println("***STATIC METHOD 1***");
		System.out.println("=======================");
		System.out.println("instance variable"+new ClassL().a);
		System.out.println("static variable"+b);
		System.out.println("=======================");
	}

	public static void main(String[] args)
	{
		System.out.println("***main METHOD***");
		System.out.println("=======================");
  }
	static
	{
		System.out.println("***STATIC METHOD  2**");
		System.out.println("=======================");
		System.out.println("instance variable"+new ClassL().a);
		System.out.println("static variable"+c);
		System.out.println("=======================");
	}

	}
PROGRAM 18:
package project2;

public class ClassR {
	
void display()
{
int a=30;
byte b=20;
float f =10.0f;

	switch(b+a)
	{
	default:
	
	System.out.println("default are execcuted");
	System.out.println("default are execcuted" +f);
	break;
	case 10:
	System.out.println("c are execcuted");
	break;
	case 20:
		System.out.println("f are execcuted");
		break;
	case 130-100:
		System.out.println("a are execcuted");
		break;
	case 40:
		System.out.println("execcuted");
	}
		
	
	}
	public static void main(String[] args) 
	{
		new ClassR().display();
	}
	}


PROGRAM 19:
package project2;

public class ClassS 
{
	void meth1()
	{
		int i=0;
		while (i<=5)
		{
			System.out.println("count===>"+i);
		i++;
		}
		System.out.println("while loop existed");
	}
	

	public static void main(String[] args)
	{

new ClassS().meth1();
	}

}

PROGRAM 20:
package project2;

public class ClassT
{
	void meth1()
	{
		int i=0;
		do
		{
			System.out.println("count===>"+i);
			i++;
		}
		while(i<=10);
		System.out.println("do while loop existed");
			}

	public static void main(String[] args) 
	{
		// TODO Auto-generated method stub
new ClassT().meth1();
	}

}
PROGRAM 21:
package project2;

public class ClassU
{
void meth1()
{
	System.out.println("**METH1**");
	System.out.println("============");
	for (int i=1;i<=10;i++) 
	{
		System.out.println("count==>"+i);
		System.out.println("============");
	}
	System.out.println("came out of for loop");
	System.out.println("============");
}

void meth2()
{
	System.out.println("**METH2**");
	System.out.println("============");
	int i=10;
	for ( System.out.println("sohel");i<=10; i++) 
	{
		System.out.println("count==>"+i);
		System.out.println("============");
	}
	System.out.println("came out of for loop");
	System.out.println("============");
}
	public static void main(String[] args)
	{
new ClassU().meth1();
new ClassU().meth2();

	}

}

PROGRAM 22:
package project2;

public class ClassV
{
void display() 
{
	int arr[]= {10,20,30,40,50,60,70,80,90,100};
	System.out.println("RETRIVING ARRAY ELEMENT USING FOR LOOP");
	System.out.println("==============================");
	for (int i=0; i<10; i++)
	{
		System.out.println(arr[i]);
	}
}
void show() 
{
	int arr[]= {10,20,30,40,50,60,70,80,90,100};
	System.out.println("RETRIVING ARRAY ELEMENT USING FOR EACH LOOP");
	System.out.println("==============================");
	for (int x:arr)
	{
		System.out.println(x);
	}
}
	public static void main(String[] args)
	{
new ClassV().display();
new ClassV().show();
	}

}

PROGRAM 23:
package project2;

public class ClassW 
{
	void meth1() 
	{
	System.out.println("there are 4 way of creating array");
	int arr1[]=new int[5];
	arr1[0]=1;
	arr1[1]=10;
	arr1[2]=100;
	arr1[3]=1000;
	arr1[4]=10000;
	arr1[5]=100000;
	arr1[6]=1000000;
	for (int i=0;i<=arr1.length;i++)
	{
		System.out.println("arr1 elements===>"+i);

	}
	}
	public static void main(String[] args) 
	{
new ClassW().meth1();
	}
	}



PROGRAM 24:
PROGRAM 25:
PROGRAM 26:
