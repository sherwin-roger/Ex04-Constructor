# Ex05-Rec-JaggedArray
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
 ### Step1: 
Start
### Step2:
Create a jagged array of 4arrays.
```
int[][] array = new int[4][];
```
### Step3:
Give the sample CPU usage in the jagged array. 
### Step4:
Print the sample CPU usage in the jagged array. 
### Step5:
stop


## Program:
```c#
using System;

class CPUactivity

{

    public static void Main(String[] args)

    {

        int[][] array = new int[4][];

        array[0] = new int[3];

        array[1] = new int[5];

        array[2] = new int[6];

        array[3] = new int[4];

        for (int i = 0; i < 4; i++)

        {

            for (int j = 0; j < array[i].Length; j++)

            {
                array[i][j] = i * j + 70;

            }

        }
        for (int i = 0; i < array.Length; i++)

        {

            for (int j = 0; j < array[i].Length; j++)

            {

                Console.WriteLine("CPU usage at node"+ i + " is "+ array[i][j]+" % ");

            }

            Console.WriteLine();

        }
    }
}
```

## Output:
![image](https://user-images.githubusercontent.com/75235488/167236657-a281d08b-cef0-416e-94bc-4bb2d0f1ece6.png)

## Result:
Thus,C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is executed successfully.
