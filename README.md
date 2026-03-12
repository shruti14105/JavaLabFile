# JavaLabFile
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
