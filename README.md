=======1=======
int a[]= {0,1,2,3,4,5,6,7,8,9,10};
        System.out.print("Array Content:");  
        for(int i=0;i<a.length;i++) 
        {
            System.out.print(" "+a[i]+", ");
        } 

=======2=======
int a[]= {0,0,0,0,0,0,0,0,0,0};
        for(int x=0;x<10;x++) {
            for(int i=0;i<a.length;i++) 
            {
                System.out.print(" "+a[i]+" ");   
            }  
            System.out.println();
        }


=======3=======
      int[] numbers = new int[]{85, 85, 85, 85, 89, 85, 85};
       //calculate sum of all array elements
       double sum = 0;
       for(int i=0; i < numbers.length ; i++){
        sum = sum + numbers[i];
        }
       //calculate average value
        double average = sum / numbers.length;
        System.out.println("Average value of the array elements is : " + average); 


=======4======= /*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package angelic_mod1;

import java.util.*;

/**
 *
 * @author hp
 */
public class Angelic_mod1 {

    public boolean endsNg(String str) {
        int len = str.length();
        String ng = "lic";
        if (len < 3) {
            return false;
        } else if (ng.equals(str.substring(len - 3, len))) {
            return true;
        } else {
            return false;
        }
    }

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Angelic_mod1 m = new Angelic_mod1();
        String str1 = "angelic";
        System.out.println("The given strings is: " + str1);
        System.out.println("The string containing ng at last: " + m.endsNg(str1));
    }

}

=======5=======
String a = "abcde";
        String b = "abc";
        System.out.println("The given string is: " + a);
        System.out.println("The given mask string is: " + b);
        char arr[] = new char[a.length()];
        char[] mask = new char[256];
        for (int i = 0; i < b.length(); i++) {
            mask[b.charAt(i)]++;
        }
        System.out.println("\nThe new string is: ");
        for (int i = 0; i < a.length(); i++) {
            if (mask[a.charAt(i)] == 0) {
                System.out.print(a.charAt(i));
                
            }
        }
        System.out.println();

=======6===========
        File my_file_dir = new File("C:\\Users\\hp\\Desktop\\array.txt");
        if (my_file_dir.exists()) {
            System.out.println("The directory or file exists.\n");
        } else {
            System.out.println("The directory or file does not exist.\n");
        }


===========7=========
  File file = new File("C:\\Users\\hp\\Desktop");
        String[] fileList = file.list();
        for (String name : fileList) {
            System.out.println(name);
        }


TABLE CLASS
.table	Adds basic styling (light padding and only horizontal dividers) to any <table>	
.table-striped	Adds zebra-striping to any table row within <tbody> (not available in IE8)	
.table-bordered	Adds border on all sides of the table and cells	
.table-hover	Enables a hover state on table rows within a <tbody>	
.table-condensed	Makes table more compact by cutting cell padding in half
.active	Applies the hover color (light-grey) to a particular row or cell	
.success	Indicates a successful or positive action	
.info	Indicates a neutral informative change or action	
.warning	Indicates a warning that might need attention	
.danger	Indicates a dangerous or potentially negative action
