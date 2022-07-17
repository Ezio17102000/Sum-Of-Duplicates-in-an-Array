# Sum-Of-Duplicates-in-an-Array

mport java.util.*;

class Main

{

public static void main(String args[])

{

Scanner sc = new Scanner(System.in);

System.out.println("Enter the size of the array");

int sum = 0;

int n = sc.nextInt();

int[] A = new int[n];

System.out.println("Enter the elements of the array");

for(int i=0;i<n;i++)

{

A[i]=sc.nextInt();

}

for(int i=0;i<n;i++)

{

for(int j=i+1;j<n;j++)

{

if (A[i]==A[j])

{

sum = sum + A[i];

}

}

}

System.out.println("Sum of duplicates is:" +sum);

}

}
