class BubbleSort {
    public static void main(String[] args) {
    int[] data = { -2, 45, 0, 11, -9 };
    // { -2, 0, 11, -9, 45 };
    // { -2, 0, -9, 11, 45 };
    // { -2, -9, 0, 11, 45 };
    //bubble sort
    int size = data.length;
    for( int i = 0; i< size ; i++) 
       for( int j =0; j< size - i - 1; j++)
           if( data [j] > data[j+1]) {
               int tmp = data[j];
               data[j] = data[ j + 1 ] ;
               data[j+1] = tmp;
           }
for( int i =0 ; i< size; i++)
  System.out.println( data[i]);
    }
}