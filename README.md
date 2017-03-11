# RecurringREAL

import java.io.FileReader;
import java.io.FileWriter;
import java.io.IOException;
import java.io.PrintWriter;
import java.util.Scanner;

public class mqin {

	public static void main(String[] args) throws Throwable {
		// TODO Auto-generated method stub

		Scanner in = new Scanner(new FileReader("fact.in"));;
		PrintWriter out = new PrintWriter (new FileWriter("fact.out"));
		
		int n = Integer.parseInt(in.nextLine());
		
		for(int i = 0; i < n; i++){
			
			int num = Integer.parseInt(in.nextLine());
			
			int f = factorial(num);
			
			out.println(f);
			
		}
		
		out.close();

	}

	
	public static int factorial(int j){
		
		if(j <= 1) return 1;
		
		return j * factorial(j - 1);
	}
	
}
