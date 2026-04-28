# JavaLabFile
[Program-1 WAP to add two distances where each distance is in m,cm,mm](#assi-1)

[Program-2 WAP to multiply with constants ](#assi-2)

[Program-3 WAP to add two distances where each distance is in m,cm](#assi-3)

[Program-4 WAP to add two times where each time is in hours,minutes,seconds](#assi-4)

[Program-5 WAP to add two times where each time is in hours,minutes](#assi-5)

[Program-6 Write a class that is having 4 methods for 1-dimensional array 1.INPUT 2.OUTPUT ORIGINAL 3.OUTPUT REVERSE 4.REVERSE](#assi-6)

[Program-7 Write a program using three classes to print 1-100 ,1-100,1-100 without  thread and analyse the output ](#assi-7)

[Program-8 Write a program using three classes to print 1-100 ,1-100,1-100 with thread and analyse the output ](#assi-8)

[Program 9- Repeat the same program 7  using runnable interface](#assi-9)

[Program 10-](#assi-10)

[Program 11- Addition of two numbers using swing](#assi-11)

[Program 12-Make a registration form with 10 elements and send the data into database (use jdbc connectivity) ](#assi-12)

[Program 13-Make one calculator in swing. ](#assi-13)

[Program 14-Matrix Addition using swing class. ](#assi-14)

[Program 15- Create one jframe apply 10 buttons on that after clicking on each button a new structure is created.(Circle, oval rectangle, etc ](#assi-15)

[Program 16-Just using mouse Event create a frame like paint brush with selection of colour and width . ](#assi-16)

[Program 17-Create a package of any 5 classes of your choice and import it.](#assi-17)

[Program 18-](#assi-18)

[Program 19-](#assi-19)

[Program 20-](#assi-20)

[Program 21-](#assi-21)

[Program 22-](#assi-22)

[Program 23-](#assi-23)





------------------

## assi-1
```
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package javaapplication31;

import java.util.Scanner;

/**
 *
 * @author IBM4
 */
public class JavaApplication31 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
      Test t1=new Test();
      Test t2=new Test();
        Test t3=new Test();
      t1.input();
      t2.input();
   
      t3.add(t1, t2);
      t3.output();
    } 
}
      class Test{

            int m,cm,mm;
              void input()
          {
              
              Scanner s = new Scanner(System.in);
               System.out.println("m=");
              m=s.nextInt();
              System.out.println("cm=");
              cm=s.nextInt();
              System.out.println("mm=");
              mm=s.nextInt();
             
          }
          void output()
          {
              System.out.println("m="+m);
              System.out.println("cm="+cm);
              System.out.println("mm="+mm);
        
        
          }
          void add(Test d1,Test d2)
          {
              m=d1.m+d2.m;
              cm=d1.cm+d2.cm;
              mm=d1.mm+d2.mm;
              if(mm>=10)
              {
                  cm=cm+1;
                  mm=mm-10;
              }
              if(cm>=100)
              {
                  m=m+1;
                  cm=cm-100;
              }
          }
          
              }
```
<img width="448" height="324" alt="image" src="https://github.com/user-attachments/assets/7cd1d40e-e645-438f-a7f3-e8a35ab46c0f" />

## assi-2
```

import java.util.Scanner;




/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author IBM4
 */
public class ABCD {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
    
  Test t1= new Test();
    Test t2= new Test();
    t1.input();
   

    t1.proc( );
 
        t1.output();

    
   
    }
}
class Test{
    int a;
    int b;
    void input(){
             Scanner s= new Scanner(System.in );
    System.out.println("a=");
    a=s.nextInt();
    System.out.println("b=") ;
    b=s.nextInt();
            
    }
    void output(){
        System.out.println("a="+a);
        System.out.println("b="+b);
        
        
    }
    void proc()
    {
        a=a*2;
        b=b*3;
       
    }
}
```
<img width="377" height="218" alt="image" src="https://github.com/user-attachments/assets/04449201-042d-465d-b89e-9ca1bcfef18d" />

## assi-3
```
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package javaapplication31;

import java.util.Scanner;

/**
 *
 * @author IBM4
 */
public class JavaApplication31 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
      Test t1=new Test();
      Test t2=new Test();
        Test t3=new Test();
      t1.input();
      t2.input();
      t3.add(t1, t2);
      t3.output();
    } 
}
      class Test{

            int m,cm;
              void input()
          {
                Scanner s = new Scanner(System.in);
               System.out.println("m=");
              m=s.nextInt();
              System.out.println("cm=");
              cm=s.nextInt();
                }
          void output()
          {
              System.out.println("m="+m);
              System.out.println("cm="+cm);
          }
          void add(Test d1,Test d2)
          {
              m=d1.m+d2.m;
              cm=d1.cm+d2.cm;
            
           
              if(cm>=100)
              {
                  m=m+1;
                  cm=cm-100;
              }
          }
          
              }
```
<img width="361" height="238" alt="image" src="https://github.com/user-attachments/assets/51d2df3a-4e71-41d2-979a-393df9f1e413" />

## assi-4
```
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package javaapplication31;

import java.util.Scanner;

/**
 *
 * @author IBM4
 */
public class JavaApplication31 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
      Test d1=new Test();
      Test d2=new Test();
        Test d3=new Test();
      d1.input();
      d2.input();
   
      d3.add(d1, d2);
      d3.output();
    } 
}
      class Test{

            int hours,minutes,seconds;
              void input()
          {
              
              Scanner s = new Scanner(System.in);
               System.out.println("hours=");
              hours=s.nextInt();
              System.out.println("minutes=");
              minutes=s.nextInt();
              System.out.println("seconds=");
              seconds=s.nextInt();
             
          }
          void output()
          {
              System.out.println("hours="+hours);
              System.out.println("minutes="+minutes);
              System.out.println("seconds="+seconds);
        
        
          }
          void add(Test t1,Test t2)
          {
              hours=t1.hours+t2.hours;
              minutes=t1.minutes+t2.minutes;
              seconds=t1.seconds+t2.seconds;
              if(seconds>=60)
              {
                  minutes=minutes+1;
                  seconds=seconds-60;
              }
              if(minutes>=60)
              {
                  hours=hours+1;
                  minutes=minutes-60;
              }
          }
          
              }
```
<img width="421" height="308" alt="image" src="https://github.com/user-attachments/assets/d00ad201-3d35-4201-8daa-92cfd5b76b72" />

## assi-5
```
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package javaapplication31;

import java.util.Scanner;

/**
 *
 * @author IBM4
 */
public class JavaApplication31 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
      Test d1=new Test();
      Test d2=new Test();
        Test d3=new Test();
      d1.input();
      d2.input();
   
      d3.add(d1, d2);
      d3.output();
    } 
}
      class Test{

            int hours,minutes;
              void input()
          {
              
              Scanner s = new Scanner(System.in);
               System.out.println("hours=");
              hours=s.nextInt();
              System.out.println("minutes=");
              minutes=s.nextInt();
              
             
          }
          void output()
          {
              System.out.println("hours="+hours);
              System.out.println("minutes="+minutes);
             
        
        
          }
          void add(Test t1,Test t2)
          {
              hours=t1.hours+t2.hours;
              minutes=t1.minutes+t2.minutes;
              if(minutes>=60)
              {
                  hours=hours+1;
                  minutes=minutes-60;
              }
          }
          
              }

```
<img width="374" height="265" alt="image" src="https://github.com/user-attachments/assets/43f0f10a-c68e-48cd-bcf4-21558dec7b8f" />


## assi-6

```
import java.util.Scanner;

class OneDArray {

    int arr[];
    int n;

    // 1. Input Method
    void input() {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter size of array: ");
        n = sc.nextInt();

        arr = new int[n];

        System.out.println("Enter elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
    }

    // 2. Original Output Method
    void displayOriginal() {
        System.out.println("Original array");
        for (int i = 0; i < n; i++) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();
    }

    // 3. Output Reverse (without changing array)
    void displayReverse() {
        System.out.println("Array in Reverse Order:");
        for (int i = n - 1; i >= 0; i--) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();
    }

    // 4. Reverse Method (actually reverse the array)
    void reverseArray() {
        int temp;

        for (int i = 0; i < n / 2; i++) {
            temp = arr[i];
            arr[i] = arr[n - 1 - i];
            arr[n - 1 - i] = temp;
        }
    }

    // Main Method
    public static void main(String[] args) {

        OneDArray obj = new OneDArray();

        obj.input();
        obj.displayOriginal();

        obj.displayReverse();

        obj.reverseArray();
       
    }
}
```
<img width="409" height="275" alt="image" src="https://github.com/user-attachments/assets/2c4a3cb5-5a6d-45c5-894a-84f70450e690" />


## assi-7
```
class ClassOne {
    void fun() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassOne " + i);
        }
    }
}

class ClassTwo {
    void fun() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassTwo " + i);
        }
    }
}

class ClassThree {
    void fun() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassThree " + i);
        }
    }
}

public class NewClass {
    public static void main(String[] args) {
        ClassOne obj1 = new ClassOne();
        ClassTwo obj2 = new ClassTwo();
        ClassThree obj3 = new ClassThree();

        obj1.fun();
        obj2.fun();
        obj3.fun();
    }
}
```
<img width="637" height="522" alt="Screenshot 2026-04-16 100728" src="https://github.com/user-attachments/assets/30577073-1831-41ff-bbe9-5618b98debe3" />


## assi-8
```
class ClassOneTh extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassOne " + i);
        }
    }
}

class ClassTwoTh extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassTwo " + i);
        }
    }
}

class ClassThreeTh extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassThree " + i);
        }
    }
}

public class NewClass1 {
    public static void main(String[] args) {
        ClassOneTh obj1 = new ClassOneTh();
        ClassTwoTh obj2 = new ClassTwoTh();
        ClassThreeTh obj3 = new ClassThreeTh();

        obj1.start();
        obj2.start();
        obj3.start();
    }
}
```
<img width="647" height="677" alt="Screenshot 2026-04-16 094708" src="https://github.com/user-attachments/assets/b0720450-0efe-4471-ab5a-0b5b434a6308" />

## assi-9
```
class ClassOneThR implements Runnable {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassOne " + i);
        }
    }
}

class ClassTwoThR implements Runnable {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassTwo " + i);
        }
    }
}

class ClassThreeThR implements Runnable {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("ClassThree " + i);
        }
    }
}

public class NewClass2 {
    public static void main(String[] args) {
        ClassOneThR obj1 = new ClassOneThR();
        ClassTwoThR obj2 = new ClassTwoThR();
        ClassThreeThR obj3 = new ClassThreeThR();

        Thread th1 = new Thread(obj1);
        th1.start();

        Thread th2 = new Thread(obj2);
        th2.start();

        Thread th3 = new Thread(obj3);
        th3.start();
    }
}
```
<img width="591" height="597" alt="runnable screenshott" src="https://github.com/user-attachments/assets/428c2233-b191-44bd-9f82-850f5d1ad704" />

## assi-10
```

```

## assi-11
```
import javax.swing.*;
import java.awt.event.*;

public class Test1 extends JFrame implements ActionListener {

    JTextField t1, t2, t3;
    JButton btn;

    Test1() {
        t1 = new JTextField();
        t2 = new JTextField();
        t3 = new JTextField();
        btn = new JButton("Add");

        t1.setBounds(50, 50, 120, 30);
        t2.setBounds(50, 100, 120, 30);
        t3.setBounds(50, 150, 120, 30);
        btn.setBounds(50, 200, 120, 30);

        add(t1); add(t2); add(t3); add(btn);

        btn.addActionListener(this);

        setSize(300, 300);
        setLayout(null);
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void actionPerformed(ActionEvent e) {
        int a = Integer.parseInt(t1.getText());
        int b = Integer.parseInt(t2.getText());
        t3.setText(String.valueOf(a + b));
    }

    public static void main(String[] args) {
        new Test1();
    }
}
```

<img width="449" height="461" alt="image" src="https://github.com/user-attachments/assets/8085c1da-8f9a-4f9b-8726-6393a42a69d2" />



## assi-12
```

```

## assi-13
```
import javax.swing.*;
import java.awt.event.*;

public class Test1 extends JFrame implements ActionListener {

    JTextField t1, t2, result;
    JButton add, sub, mul, div;

    Test1() {
        t1 = new JTextField();
        t2 = new JTextField();
        result = new JTextField();

        add = new JButton("+");
        sub = new JButton("-");
        mul = new JButton("*");
        div = new JButton("/");

        t1.setBounds(50,50,100,30);
        t2.setBounds(50,100,100,30);
        result.setBounds(50,150,100,30);

        add.setBounds(200,50,50,30);
        sub.setBounds(200,100,50,30);
        mul.setBounds(200,150,50,30);
        div.setBounds(200,200,50,30);

        add(t1); add(t2); add(result);
        add(add); add(sub); add(mul); add(div);

        add.addActionListener(this);
        sub.addActionListener(this);
        mul.addActionListener(this);
        div.addActionListener(this);

        setSize(350,300);
        setLayout(null);
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void actionPerformed(ActionEvent e) {
        int a = Integer.parseInt(t1.getText());
        int b = Integer.parseInt(t2.getText());

        if (e.getSource() == add)
            result.setText(String.valueOf(a+b));
        else if (e.getSource() == sub)
            result.setText(String.valueOf(a-b));
        else if (e.getSource() == mul)
            result.setText(String.valueOf(a*b));
        else if (e.getSource() == div)
            result.setText(String.valueOf(a/b));
    }

    public static void main(String[] args) {
        new Test1();
    }
}
```

<img width="530" height="450" alt="image" src="https://github.com/user-attachments/assets/80029d58-7ea6-4d88-bd38-72c3b75cd058" />


## assi-14
```
import javax.swing.*;
import java.awt.event.*;

public class Test1 extends JFrame implements ActionListener {

    JTextField a1,a2,a3,a4,b1,b2,b3,b4,r1,r2,r3,r4;
    JButton btn;

    Test1() {
        setLayout(null);

        a1=new JTextField(); a2=new JTextField();
        a3=new JTextField(); a4=new JTextField();

        b1=new JTextField(); b2=new JTextField();
        b3=new JTextField(); b4=new JTextField();

        r1=new JTextField(); r2=new JTextField();
        r3=new JTextField(); r4=new JTextField();

        btn=new JButton("Add");

        a1.setBounds(50,50,40,30); a2.setBounds(100,50,40,30);
        a3.setBounds(50,100,40,30); a4.setBounds(100,100,40,30);

        b1.setBounds(200,50,40,30); b2.setBounds(250,50,40,30);
        b3.setBounds(200,100,40,30); b4.setBounds(250,100,40,30);

        r1.setBounds(350,50,40,30); r2.setBounds(400,50,40,30);
        r3.setBounds(350,100,40,30); r4.setBounds(400,100,40,30);

        btn.setBounds(200,150,100,30);

        add(a1);add(a2);add(a3);add(a4);
        add(b1);add(b2);add(b3);add(b4);
        add(r1);add(r2);add(r3);add(r4);
        add(btn);

        btn.addActionListener(this);

        setSize(500,300);
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void actionPerformed(ActionEvent e) {
        r1.setText(""+(Integer.parseInt(a1.getText())+Integer.parseInt(b1.getText())));
        r2.setText(""+(Integer.parseInt(a2.getText())+Integer.parseInt(b2.getText())));
        r3.setText(""+(Integer.parseInt(a3.getText())+Integer.parseInt(b3.getText())));
        r4.setText(""+(Integer.parseInt(a4.getText())+Integer.parseInt(b4.getText())));
    }

    public static void main(String[] args) {
        new Test1();
    }
}
```
<img width="751" height="443" alt="image" src="https://github.com/user-attachments/assets/611c6666-09d7-41fe-862e-f9042d118dbb" />

## assi-15
```
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

public class Test1 extends JFrame implements ActionListener {

    String shape="";

    JButton circle, rect, oval;

    Test1() {
        circle=new JButton("Circle");
        rect=new JButton("Rectangle");
        oval=new JButton("Oval");

        circle.setBounds(50,50,100,30);
        rect.setBounds(160,50,100,30);
        oval.setBounds(270,50,100,30);

        add(circle); add(rect); add(oval);

        circle.addActionListener(this);
        rect.addActionListener(this);
        oval.addActionListener(this);

        setSize(500,400);
        setLayout(null);
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void actionPerformed(ActionEvent e) {
        shape = e.getActionCommand();
        repaint();
    }

    public void paint(Graphics g) {
        super.paint(g);

        if(shape.equals("Circle"))
            g.drawOval(200,150,100,100);
        else if(shape.equals("Rectangle"))
            g.drawRect(200,150,120,80);
        else if(shape.equals("Oval"))
            g.drawOval(200,150,150,80);
    }

    public static void main(String[] args) {
        new Test1();
    }
}
```
<img width="769" height="614" alt="image" src="https://github.com/user-attachments/assets/a2dfbe97-345a-4803-881d-ccd71b74d3f6" />


## assi-16
```
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

public class Test1 extends JFrame implements MouseMotionListener {

    int x,y;

    Test1() {
        addMouseMotionListener(this);
        setSize(500,400);
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public void mouseDragged(MouseEvent e) {
        Graphics g = getGraphics();
        g.fillOval(e.getX(), e.getY(), 5, 5);
    }

    public void mouseMoved(MouseEvent e) {}

    public static void main(String[] args) {
        new Test1();
    }
}
```
<img width="755" height="592" alt="image" src="https://github.com/user-attachments/assets/825eedbb-b657-48fc-88fd-2e3c6a48bb7e" />


## assi-17
```

```

## assi-18
```

```
## assi-19
```
public class Test1 {
    public static void main(String[] args) {

        try {
            int arr[] = {1,2,3,4,5};
            System.out.println(arr[10]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Array index out of bounds!");
        }

        try {
            int a = 10/0;
        } catch (ArithmeticException e) {
            System.out.println("Division by zero not allowed!");
        }
    }
}
```

<img width="1051" height="489" alt="image" src="https://github.com/user-attachments/assets/747bfded-a279-4027-b082-b08fc32e7fdf" />

## assi-20
```
class AgeException extends Exception {
    AgeException(String msg) {
        super(msg);
    }
}

public class Test1 {
    static void checkAge(int age) throws AgeException {
        if(age < 18)
            throw new AgeException("Invalid Age!");
        else
            System.out.println("Valid Age");
    }

    public static void main(String[] args) {
        try {
            checkAge(15);
        } catch(Exception e) {
            System.out.println(e);
        }
    }
}
```

<img width="1174" height="639" alt="image" src="https://github.com/user-attachments/assets/0e88e24e-41df-4294-95eb-ffdd87bd1fc1" />



## assi-21
```
import java.io.*;

public class Test1 {
    public static void main(String[] args) {
        try {
            FileWriter fw = new FileWriter("test.txt");
            fw.write("Hello File");
            fw.close();

            BufferedReader br = new BufferedReader(new FileReader("test.txt"));
            System.out.println(br.readLine());
            br.close();

        } catch(Exception e) {
            System.out.println(e);
        }
    }
}
```
<img width="878" height="540" alt="image" src="https://github.com/user-attachments/assets/7cca62d3-46d8-4f6d-813b-89cc28e7291e" />

## assi-22
```

```






