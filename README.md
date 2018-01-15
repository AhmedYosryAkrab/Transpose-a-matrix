# Transpose-a-matrix
How to transpose a matrix by a Java code

package Lab;
import java.util.Scanner;
public class Transpose {

	public static void main(String[] args) {
		int m;
		int n;
		
		Scanner sc = new Scanner(System.in);
		m = sc.nextInt();
		n = sc.nextInt();
		int [][]matrix1 = new int [m][n];
        int [][]matrix2 = new int [n][m];
        for(int i=0 ; i<m ; i++){
        	for(int j=0 ; j<n ; j++){
        		matrix1[i][j] = sc.nextInt();
        	}
        }
	  for(int i=0 ; i<m ; i++){
		for(int j=0 ;j<n ; j++){
			matrix2[j][i] = matrix1[i][j];
		}
	}
	  for(int i=0;i<n;i++){
		  for(int j=0; j<m;j++){
			 System.out.print(matrix2[i][j]+"\t");
		  }
		  System.out.println();
	  }
	}

}
