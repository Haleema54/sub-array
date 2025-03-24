# sub-array
public class Main
{
    public static int[] substring(){
        int[] nums={1,2,3,4,5};
        return nums;
    }
	public static void main(String[] args) {
	    int[] sub=substring();
	    for(int i=0;i<sub.length;i++){
	        for(int j=i;j<sub.length;j++){
	            for(int k=i;k<j;k++){
	                System.out.print(sub[k]);
	            }
	            System.out.println();
	        }
	        
	    }
	}
}
# output
1
12
123
1234
12345
2
23
234
2345
3
34
345
4
45
5
# sub array with k nums:
public class Main
{
    public static int[] substring(){
        int[] nums={1,2,3,4,5};
        return nums;
    }
	public static void main(String[] args) {
	    int[] sub=substring();
	    int l=3;
	    int n=sub.length;
	    for(int i=0;i<n-l+1;i++){
	        for(int j=n-l+1;j<=n;j++){
	            for(int k=i;k<j;k++){
	                System.out.print(sub[k]);
	            }
	            i++;
	            System.out.println();
	        }
	        
	    }
	}
}
#output:
123
234
345
