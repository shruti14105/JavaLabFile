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
img width="637" height="522" alt="Screenshot 2026-04-16 100728" src="https://github.com/user-attachments/assets/06d4906a-04cb-425b-8777-344a6a406d7e" /><


