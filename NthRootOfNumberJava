/*package whatever //do not write package name here */

import java.io.*;
class GFG {
    private static double multiply(double number, int n) {
        double ans = 1.0;
        for(int i = 1;i<=n;i++) {
            ans = ans * number;
        }
        return ans; 
    }
    private static void getNthRoot(int n, int m) {
        double low = 1;
        double high = m;
        double eps = 1e-6; 
        
        while((high - low) > eps) {
            double mid = (low + high) / 2.0; 
            if(multiply(mid, n) < m) {
                low = mid; 
            }
            else {
                high = mid; 
            }
        }
        
        System.out.println(low + " " + high);  
        
        // just to check
         System.out.println(Math.pow(m, (double)(1.0/(double)n))); 
    }
	public static void main (String[] args) {
		int n = 17, m = 89; 
		getNthRoot(n, m); 
	}
}
