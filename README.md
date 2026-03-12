# JavaLabFile
[Program-1 WAP to add two distances where each distance is in m,cm,mm](#assi-1)

[Program-2 WAP to multiply with constants ](#assi-2)

[Program-3 WAP to add two distances where each distance is in m,cm](#assi-3)

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
          
      
// TODO code application logic here
```
<img width="361" height="238" alt="image" src="https://github.com/user-attachments/assets/51d2df3a-4e71-41d2-979a-393df9f1e413" />


