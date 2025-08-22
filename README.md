//ARRAY
//Array is a collection of similar datatype element.


import java.util.Scanner;
class Array 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int A[] = new int[3],i;
        int B[]= new int[3];
        int Merge[] = new int[6];
        int x = 3;

        System.out.println("Enter 3 elements in A[]:");

        for ( i = 0; i < 3; i++) 
        {
            A[i] = sc.nextInt();
        }

        System.out.println("Enter 3 elements in B[]:");
        for ( i = 0; i < 3; i++) 
        {
            B[i] = sc.nextInt();
        }

        for ( i = 0; i < 3; i++) 
        {
            Merge[i] = A[i];
        }

        for ( i = 0; i < 3; i++) 
        {
            Merge[x] = B[i];
            x++;
        }

        System.out.println("Merged Array:");
        for ( i = 0; i < 6; i++) 
        {
            System.out.print(Merge[i] + " ");
        }
    }
}


//Binary 
/*
import java.util.Scanner;
class Binary 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int[] A = new int[10];
        int key, l = 0, u = 9, m;
        Boolean flag = false;

        System.out.println("Enter Values in A[]:");
        for (int i = 0; i < 10; i++) 
        {
            A[i] = sc.nextInt(); 
        }

        System.out.println("Enter Key Value");
        key = sc.nextInt();

        while(l<=u)
        {
            m = (l+u)/2;

            if(key>A[m])
            {
                l = m + 1;
            }

            else if(key<A[m])
            {
                u = m - 1;
            }

            else
            {
                flag = true;
                break;
            }
        }

        if(flag)
        {
            System.out.println("Value Found");
        }
        else
        {
            System.out.println("Value Not Found");
        }
    }
}
*/