Create a Class Medicine with the below attributes:

medicineName - String
batchNo - String
disease - String
price - int

Write getters, setters and parameterized constructor as required. 

Public class Solution is already created with main method.
Code inside main method should not be altered else your solution might be scored as zero.
You may copy the code from main method in eclipse to verify your implementation.

Implement static method - medicinePriceForGivenDisease in Solution class.

This method will take a String parameter named disease along with the other parameter as array of Medicine objects. 
The method will return an array of Integer containing the price of the medicines in ascending order, if the given input(disease) matches the disease attribute of the medicine objects in the Array.

Note : 1) Same disease can have more than one medicine.
2) disease search should be case insensitive.

This method should be called from the main method and display the prices.

Main method mentioned above already has Scanner code to read values, create objects and test above methods. Hence do not modify it.

Consider below sample input and output:

Input:
Hyadry
FHW0602
EyeDryness
140
Dolo
FHW0603
Fever
10
OpsionHA
P5011
EyeDryness
435
Mucinex
C0011
Cold
15
EyeDryness

Output:
140
435

-------------------------------------------------------------------------
Sample code snippet for reference:
Please use below code to build your solution.
Make sure that Solution class is public and Medicine class is not public.
--------------------------------------------------------------------------
import java.util.Scanner;

public class Solution {
public static void main(String[] args) {
Medicine[] medicine = new Medicine[4];
String search;

Scanner sc = new Scanner(System.in);

for (int i = 0; i < medicine.length; i++) {
String medicineName = sc.nextLine();
String batchNo = sc.nextLine();
String disease = sc.nextLine();
int price = sc.nextInt();
sc.nextLine();
medicine[i] = new Medicine(medicineName, batchNo, disease, price);

}

search = sc.nextLine();
Integer[] price = medicinePriceForGivenDisease(medicine, search);

for(int i=0;i<price.length;i++) {
System.out.println(price[i]);
}
}
public static Integer[] medicinePriceForGivenDisease(Medicine[] medicine,String disease)
{
//method logic
//code to find price, sort and return the sorted array.
}
}

class Medicine
{
//code to build Medicine class
}













              
import java.util.Scanner;

public class Solution {
 public static void main(String[] args) {
  Medicine[] medicine = new Medicine[4];
  String search;

  Scanner sc = new Scanner(System.in);

  for (int i = 0; i < medicine.length; i++) {
   String medicineName = sc.nextLine();
   String batchNo = sc.nextLine();
   String disease = sc.nextLine();
   int price = sc.nextInt();
   sc.nextLine();
   medicine[i] = new Medicine(medicineName, batchNo, disease, price);

  }

  search = sc.nextLine();
  Integer[] price = medicinePriceForGivenDisease(medicine, search);
  
  for(int i=0;i
          

Instruction : 
Kindly mention class name as MyClass.
