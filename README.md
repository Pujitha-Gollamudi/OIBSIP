# task_2
import java.util.Random;   
import java.util.*;
	public class Game{
	public static void main(String args[]){
		int ch=1;
		int c=1;
		Scanner Sc=new Scanner(System.in);
		while(ch > 0){
		c=1;
		System.out.println("Enter low limit Value:");
		int min=Sc.nextInt();
		System.out.println("Enter high limit Value:");
		int max=Sc.nextInt();
		int R=(int)(Math.random()*max-min+1);   
		System.out.print("Enter positive Number:");
		int N=Sc.nextInt();
		while(N!=R){
			c++;
			if(N<R){
				System.out.println("   "+N+"  is smaller");
			}
			if(N>R){
				System.out.println("   "+N+"  is greater");
			}
			
			System.out.print("Enter another number: ");
			N=Sc.nextInt();
			
		}
		System.out.println("\n");
		if(c==1)System.out.println("   * * * * *\n   Congrats!!!");
		else if(c==2)System.out.println("   * * *\n   Congrats!!");
		else if(c==3)System.out.println("   *\n   Congrats!");
		else System.out.println("Won");
		System.out.println("   You gussed the number in " +c+"  chances");
		System.out.println("Do you want to continue!!!");
		System.out.println("If yes enter a positive number\nElse enter a negative number: ");
		ch=Sc.nextInt();
		}
	}
}

