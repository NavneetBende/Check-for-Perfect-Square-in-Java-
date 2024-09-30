Check for Perfect Square in Java
Here on this page, we will learn how to Check for Perfect Square in Java programming language. We are given an integer number and need to print “True” if it is, otherwise “False”.

Check for Perfect Square
Algorithm ( Method 1 )
Take the floor() value square root of the number.
Multiply the square root twice.
We use the Boolean equal operator to verify if the product of the square root is equal to the number given.
Check for Perfect Square in Java
Java Code
Run
public class Main {

	static boolean isPerfectSquare(int x)
	{
		if (x >= 0) {
		
			int sr = (int)Math.sqrt(x);
		
			return ((sr * sr) == x);
		}
		return false;
	}

	public static void main(String[] args)
	{
		int x = 84;

		if (isPerfectSquare(x))
			System.out.print("True");
		else
			System.out.print("False");
	}
}
Output
False
Algorithm ( Method 2 )
In this method we use the floor and ceil function.
If they are equal that implies the number is a perfect square.
Run
import java.io.*;

public class Main{

static void checkperfectsquare(int n)
{
	
	if (Math.ceil((double)Math.sqrt(n)) == Math.floor((double)Math.sqrt(n)))
	{
		System.out.print("True");
	}
	else
	{
		System.out.print("False");
	}
}

public static void main(String[] args)
{
	int n = 49;
	
	checkperfectsquare(n);
}
}
Output
True
