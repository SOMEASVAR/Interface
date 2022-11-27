# Interface

## Aim:
To Develop a small bank application by declaring deposit() and withdrawal() as abstract methods in the interface. Get the choice from the user whether to perform withdrawal or deposit operation. After the operation completes, display the balance amount.


## Algorithm:
## Step 1:
Create an Interface.

## Step 2:
Create a child class.

## Step 3:
Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.

## Step 4:
Create those 2 functions in the child class and perform respective operation.

## Step 4:
Use while loop and and switch case to Get the choice from the user whether to perform withdrawal or deposit operation.

## Step 5:
After performing the functions display the remaining balance of the user.


## Program:
```
using System;
namespace iiinterface
{
    class Program
    {
        public interface bank
        {
            void deposit(int amount);
            
            void withdrawl(int amount);
        }
        public class bankEX
        {
            int balance = 5000;
            public void deposit(int amount)
            {
                balance+=amount;
                Console.WriteLine(balance);
            }
            public void withdrawl(int amount)
            {
                balance-=amount;
                Console.WriteLine(balance);
                
            }
            public static void Main()
            {
                bankEX obj = new bankEX();
                Console.WriteLine("1.Deposit\n2.Withdrawl");
                int ch = Convert.ToInt32(Console.ReadLine());
                if(ch == 1)
                {
                    Console.WriteLine("Enter the amount you want to Deposit:");
                    int amount = Convert.ToInt32(Console.ReadLine());
                    Console.WriteLine("Your Balance amount is:");
                    obj.deposit(amount);
                }
                else if(ch == 2)
                {
                    
                    Console.WriteLine("Enter the amount you want to Withdraw:");
                    int amount = Convert.ToInt32(Console.ReadLine());
                    Console.WriteLine("Your Balance amount is:");
                    obj.withdrawl(amount);
                }

            }
        }
    }
}
```


## Output:

![inter](https://user-images.githubusercontent.com/93434149/204127814-213beeaf-c192-4fd1-a974-cc54fabf2e8d.jpg)


## Result:
C# program to develop a bank application using interface is implemented successfully.
