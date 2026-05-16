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
