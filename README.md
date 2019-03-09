# helloworld
this is a exercise
public static void main()

this is a exercise
public static void main()

this is a exercise
public static void main()

public static void sort(int[] arr,int low,int high){
        if (low>=high){
            return;
        }
        int i = low;
        int j = high;
        int key = arr[i];
        while (i<j){
            while (arr[j]>=key && i<j){
                j--;
            }
            int t;
            t = arr[i];
            arr[i] = arr[j];
            arr[j] = t;

            while (arr[i]<=key && i<j){
                i++;
            }
            t = arr[i];
            arr[i] = arr[j];
            arr[j] = t;

            sort(arr,low,i-1);
            sort(arr,i+1,high);
        }
    }
