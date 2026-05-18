# java-daily-practice-dsaa
#LINEAR SEARCH 
public class Main{
public static void main(String[] args){
int[] arr={4,2,5,1,9};
int target=1;
int index=-1;
for(int i=0;i<arr.length;i++){
if(arr[i]==target){
index=i;
break;
}
}
System.out.println(index);
}//oUtput :- 3 
}

#BINARY SEARCH 
public class Main{
public static void main(String[] args){
int[] arr={1,3,5,7,9};
int target = 7;
int low=0,high=arr.length-1;
int index=-1;
while(low<= high){
int mid=(low+high)/2;
if(arr[mid]==target){
index=mid;
break;
} else if(arr[mid]<target){
low=mid+1;
} else{
high=mid-1;
}
}
System.out.println(index);
}
}


















#MAXIMUM & MINIMUM ARRAYS
public class Arrays {
    public static void main(String[] args) {
        int[] arr = {4, 2, 3, 1, 9, 7};
        int max = arr[0];
        int min = arr[0];
        for (int i = 1; i < arr.length; i++) {
            if (arr[i] > max) {
                max = arr[i];
            }
            if (arr[i] < min) {
                min = arr[i];
            }
        }
        System.out.println("Max = " + max);
        System.out.println("Min = " + min);
    }
} //Max=9,Min=1


#REvERSE ARRAY 
import java.util.Arrays;
public class ReverseArrays {
    public static void main(String[] args) {
        int[] arr = {1, 2, 3, 4, 5};
        int start = 0;
        int end = arr.length - 1;
        while (start < end) {
            int temp = arr[start];
            arr[start] = arr[end];
            arr[end] = temp;
            start++;
            end--;
        }
        System.out.println(Arrays.toString(arr));
    }
}



#
