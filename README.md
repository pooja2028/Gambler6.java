# Gambler6.java
import java.util.*;
public class Gambleruc4 {
	static int stakePerDay = 100; //stake is in dollar
	static int betPerGame =  1 ; 
	static int totalStake = 100;
	static int chancePerDay = 100;
	static int days = 20;

	public static void main(String[] args)
	{
		for (int i = 1; i <= 20; i++) {
			for (int j = 1; j <= chancePerDay; j++) {
				Random random= new Random();  
				int bet = random.nextInt(2);

				if (bet==1)
					totalStake ++;
				else
					totalStake--;


				totalStake=totalStake+100;
			}
		}
		System.out.println("Total Amount after 20 days "+totalStake);
	}
}
