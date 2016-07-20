# TragetFindBySumTwoInteger
import java.util.Scanner;


public class AddTwoIntegerInArray {

	public static void main(String[] arg) {
		int a = 0, k = 0;
		int l = 0;
		Scanner qq = new Scanner(System.in);
		System.out.println("Enter array size");
		int nn=qq.nextInt();
		int count[] = new int[nn];
			System.out.println("Enter array element");
		for(int i=0;i<nn;i++)
		{
			count[i]=qq.nextInt();
		}
		int sum;
		System.out.println("Enter the target");;
		int target=qq.nextInt();
		int ind=0;
		for(int i=0;i<nn;i++)
		{
			for(int j=i+1;j<nn;j++)
			{
				sum=0;
				sum=count[i]+count[j];
				if(sum==target)
				{
					ind=1;
					break;
				}
			}
			
		}
		if (ind == 1) {
			System.out.println("Traget is sum of integer");
		} else
			System.out.println("not");
	}
}
