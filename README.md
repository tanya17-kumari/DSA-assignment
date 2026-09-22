           ASSIGNMENT:1

(1) Program to point "Dsa" 5 times 

      program 
#include<stdio.h>
int main() {
   int I;
   for(I=1; I<=5; I++)
{
   printf("DSA\n");
}
   return 0;
}

        OUTPUT 
DSA
DSA
DSA
DSA
DSA

(2) Checking for loop

      PROGRAM 
#include<stdio.h>
int main() {
   int I;
   for(I=1; I<=10; I++)
{
   printf(" %d ", i);
}
   return 0;
}

       OUTPUT 
1 2 3 4 5 6 7 8 9 10

(3) *
    * *
    * * * 
    * * * *

         PROGRAM 
#Include<stdio.h>
int main() {
    int num;
    printf("Enter number of rows:");
    scanf(" %d" , & num);
    for(int I=1;i<= num;i++){
    for(int j=1; j<=i; j++){
        printf("*");
    }
    printf("\n");
  }
    return 0;
}

          OUTPUT 
  *
  * *
  * * *
  * * * * 


  (4) * * * * 
      * * *
      * * 
      *

             PROGRAM 
#Include<stdio.h>
 int main() {
    int num;
    printf("Enter number of rows:");
    scanf(" %d" , & num);
    for(int I=num;i>=1;i--){
    for(int j=1; j<=i; j++){
        printf("*");
    }
        printf("\n");
  }
    return 0;
}

          OUTPUT 
  * * * * 
  * * * 
  * *
  * 



        ASSIGNMENT:2

5) Factorial using recursion + Iteration.

=>                  Program

#include <stdio.h>
int factorial (int n) {
    if (n == 0 || n == 1)return 1;
    }
    return (n * factorial(n-1));
}

int main() {
    int a = 5;
    printf("%d! = %d", a,factorial(a));
}

           OUTPUT 
5!=120

6) Identifying Types of data Structure (Array, Linked List, Tree, Graph).

                    Program
#include <stdio.h>
#include <string.h>
 int main() {
    char dsName[20];
printf("Enter name(Array,LL,Tree,Graph): ");
       scanf("%s", dsName);
if(strcmp(dsName,"Array") == 0 || strcmp(dsName,"LL")== 0) {
printf("%s is a LINEAR Data structure\n", distance);
}
   else if (strcmp(dsName, "Tree") == 0 || strcmp(dsName,"Graph") == 0) {
printf("%s is a NON-LINEAR data structure.\n", dsName);
}
else {
printf("Unknown data structure!\n");
}
    return 0;
}

            OUTPUT 
i) Enter name (Array, LL, Tree, Graph): Array
   Array is a LINEAR data structure.

ii) Enter name (Array, LL, Tree, Graph): Stack
    Unknown data structure!

iii) Enter name (Array, LL, Tree, Graph): Tree
     Tree is a NON-LINEAR data structure.

iv) Enter name (Array, LL, Tree, Graph): Array_list
    Unknown data structure!


(7)Input one 1-D Array, one 2-D Array.
    •Access 1 element from both,
    •Traversing of both.

             Program
#include <stdio.h>
int main() {
    int arr 1D [3] = {10,20,30};
      int arr 2D [2][2] = {{1,2}, {3,4}};
      int i, j ;
         printf ("Accessing 1-D element : %d\n", arr 1D [1]);
         printf ("Accessing 2-D element : %d\n\n", arr 2D [0][1]);
         printf ("Traversing 1-D Array:\n");
         for (i = 0 ; i < 3; i++) {
            printf ("%d", arr 1D [i]);
 }
    printf ("\n\n");
    printf ("Traversing 2-D Array:\n");
    for (i = 0 ; i < 2 ; i++) {
    for (j = 0 ; j < 2 ; j++) {
    printf ("%d", arr 2D [i][j]);
}
  printf ("\n");
}
 return 0;
}
 

         OUTPUT 

Accessing 1-D element : 20
Accessing 2-D element : 4
Traversing 1-D Array:
        10 20 30
Traversing 2-D Array:
          1   2
          3   4


          ASSIGNMENT:3 

Q(8)Insert an element in an array using function.
            
            PROGRAM
#include <stdio.h>
void insert (int arr [],int size, int pos, int item) {
for (int i= size ; i > pos ; i-- ) {
      arr [i]= arr [i-1];
}
     arr [pos]= item ;
   (*size) ++;
}
  void display (int arr [], int size) {
  for (int i=0 ; i < size ; i++) {
      printf (" %d" , arr [i]);
}
    printf (" \n ");
}
  int main ( ) {
  int arr [10]= {10,20,30,40,50};
  int size = 5 ;
  int pos = 2 ; item= 99 ;
  printf (" Before: ") ;
  display (arr, size);
  insest (arr, & size, pos, item) ;
  printf (" After: ") ;
  display (arr, size);
  return 0 ;
}
     
           OUTPUT 
Before:
10 20 30 40 50
After:
10 20 99 30 40 50

Q(9) Delete an element from an array using function.

             
             PROGRAM 
#include <stdio.h>
void display(int arr[], int size) {
    for (int i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
}
void delete Element(int arr[], int *size, int pos) {
    for (int i = pos; i < *size - 1; i++) {
        arr[i] = arr[i+1];
    }
    (*size)--;
}
int main() {
    int arr[20] = {10, 20, 30, 40, 50};
    int size = 5;
    int pos = 2;
    printf("Before delete:\n");
    display(arr, size);
    delete Element(arr, &size, pos);
    printf("After delete:\n");
    display(arr, size);
    return 0;
}


          Output

Before delete:10 20 30 40 50
After delete:10 20 40 50

Q(10)Write linear search using function.

              PROGRAM 
# include <stdio.h>
int linearSearch (int arr [ ], int size , int key) {
  for (int i=0 ; i<size ; i++){
    if (arr [i] == key) {
       return 1;
    }
  }
  return -1;
}
void display Result (int index, int key){
    if (index != -1) {
       printf (" Sucess : element %d found at index %d.\n",key,index );
    }
    else {
       printf (" failure : element %d not found at index %d \n", key , index );
    }
}
void run program ( ){
     int arr [ ] = { 12,45,7,91,30 }
     int size = 5;
     int Key = 91;
     int result Index = linearsearch (arr, size, key);
     displayResult (resultIndex, key);
}
int main ( ) {
    runProgram ( ) ;                    Output
    return 0;   
}                                                   

           OUTPUT 
Success : Element 91 found at index 3
    
Q(11)write Binary Search (Iterative) using function.
   
            PROGRAM 
#include <stdio.h>
   int binarySearch (int arr[], int size, int key) {
   int low = 0; high = size - 1;
   while (low <= high) {
   int mid = low + (high - low) / 2;
   if (arr[mid] == key) return mid;
   else if (arr[mid] < key) low = mid + 1;
   else high = mid - 1;
}
return -1;
}
    void display (int res, int key) {
       if (res != -1) printf ("found %d at index %d\n", key, res);
     else printf ("%d not found\n", key);
     void run () {
     int arr[] = {10, 20, 30, 40, 50};
     int size = 5; key = 40;
     display (binarySearch (arr, size, key), key);
}
   int main() {
run();
return 0;
}
       
       OUTPUT 
Found 40 at index 3


Q(12)write Binarysearch (Recursive) using function.
            
            
            PROGRAM 
#include<stdio.h>
int binarysearch(int arr[],int low, int high, int key){
    if (low > high) {
        return -1;
    }
    int mid = low + (high - low) / 2;
    if (arr[mid] == key){
        return mid;
    }
    else if (arr[mid] < key){
        return binarysearch(arr, mid + 1, high, key);
    }
    else {
        return binarysearch(arr, low, mid - 1, key);
    }
}
int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int size = 5;
    int key = 40;
    int result = binarysearch(arr, 0, size - 1, key);
    if (result != -1) {
        printf("Element found at index %d\n", result);
    } else {
        printf("Element not found at index %d\n", result);
    }
    return 0;
}



           OUTPUT 
Element found at index 3


            ASSIGNMENT: 4
Q(13) Q.1) write a C program for playing with pointers using a pointer and a double pointer.


           PROGRAM 
#include <stdio.h>
   int main () {
   int age = 25;
   int * p = & age ;
   int ** pp = & p ;
   printf ( "%d , %d , %d" , age , * p , ** pp ) ;
  (*p) ++ ;
  printf ( "%d , %d" , age , **pp ) ;
  ** pp += 10 ;
  printf ( "%d , %d , %d" , age , * p , ** pp ) ;
  int x = 50 ;
  * pp = & x ;
  printf ( "%d , %d , %d" , age , * p , ** pp ) ;
  (*P) = 45 ;
  printf ( "%d / %d , %d , %d" , x , * P , ** PP ) ;
  printf ( "%d , %d" , age , x ) ;
  return 0 ;
}


         OUTPUT 
25, 25, 25
26, 26
36, 36, 36
36, 50, 50
45, 45, 45
36, 45


Q.(14) write a C program to access 1 element of an array using pointer.


           PROGRAM 
#include <stdio.h>
int main () {
int arr, n , i , pos;
printf ( "Enter number of elements: " ) ;
scanf ( "%d" , & n ) ;
printf ( "Enter elements : " ) ;
for ( i = 0 ; i < n ; i++ )
scanf ( "%d" , & arr [i] ) ;
printf ("Enter position to access: ");
      scanf ("%d", &pos);
      printf ("Element: %d\n", *(arr + pos));
      printf ("& Found at index = %d", pos);
      return 0;
}
   3

             Output
enter number of elements
Enter elements : 1 2 4
Enter position to access : 1
Element = 7
found at index = 1



Q(15) write a c program to traververse an array using pointer

          PROGRAM 
#include<stdio.h>
   void traversearray (int *arr, int size) {
   for (int i = 0; i < size ; i++) {
   printf ("Elements at index %d: %d, \n", i , arr);
    }
 }
        int main () {
        int array[ ] = {10, 20, 30, 40, 50};
        int length = size of (array) / size of (array [0]);
        printf ("Traversing the array using function ");
        traversearray (array, length);
        return 0;
}

           OUTPUT 
Traversing the array using function:
Element at index 0: 10;
Element at index 1: 20;
Element at index 2: 30;
Element at index 3: 40;
Element at index 4: 50;

Q(16)Write a c program linear search using pointer 

            PROGRAM 
#include <stdio.h>
   int linearsearch(int arr[],int size,int key){ 
   for (int i = 0 ; i < size ; i++) 
   if (arr+i== key) {
   return i;  
  }
}
    return -1;
}
   int main(){
   int Arr [10]= {1, 2, 3, 4, 5, 6, 7, 8, 9};
    int size = size of (Arr) /size of (Arr [0]);
    int key = 5;
    int result = linearsearch(Arr, size, key);
    if(result != -1){
    printf("Element %d found at index:%d \n",key,result);
} else {
        printf("Element %d not found.\n",key);
  }
    return 0;
}


               OUTPUT 
Element 5 found at index: 4


Q(17) Write a program about switch case to calculate addition of 2D array.

            PROGRAM 
#include <stdio.h>
int main(){
    int choice, W, I, J, LR, LC, n, N;
    long B, address,
    printf("Press 1 for Row major.\n");
    printf("Press 2 for column major.\n");
    printf("Enter your choice: ");
    scanf("%d", & choice);
    printf("Enter Base address (B) : ");
    scanf("%ld", &B);
    printf("Enter size of each element in bytes(w) : ");
    scanf("%d", &w);
    printf("Enter Row index (I) : ");
    scanf("%d", &I);
    printf("Enter column index(J) : ");
    scanf("%d", &J);
    printf("Enter lowest row index (LR) : ");
    scanf("%d", &LR);
    printf("Enter lowest column index (LC) : ");
    scanf("%d", &LC);
    printf("Enter total number of Rows (n) : ");
    scanf("%d", &n);
    printf("Enter total number of columns (N) : ");
    scanf("%d", &N);
    switch (choice) {
        case 1:
            address = B + w * ((I - LR) * N + (J - LC));
            printf("Address in Row-major : %ld \n", address);
            break;
        case 2:
        address = B + w * ((J - LC) * n + (I - LR));
        printf("Address in col-major : %ld \n", address);
        break;
        default:
        printf("Invalid choice.\n");
    }
    return 0;
}

           OUTPUT 
Press 1 for Row major ,
Press 2 for column major,
Enter your choice : 2
Enter Base address (B) : 1600
Enter size of each element in bytes (w) : 4
Enter Row index (I) : 2
Enter column index (J) : 2
Enter lowest column index (LC) : 0
Enter lowest row index (LR) : 0
Enter total number of Rows(n) : 3
Enter total number of Columns(N) : 4
Address in column major : 1632


           ASSIGNMENT:5 
Q(18)Implement bubble Sort


             PROGRAM 
#include <stdio.h>
  void bubblesort (int array[], int size){
  int step, i;
  for (step = 0; step < size -1; step ++){
  for (i = 0; i < size -step-1; i++){
        if (array [i] > array [i + 1]){
            int temp = array [i];
            array [i] = array [i+1];
             array [i+1] = temp;
       }
}
        for (i=0; i < size ; i++){
        printf ("%d", array[i]);
 }
        Printf ("\n");
    }
}
  int main(){
    int i;
    int data [] = {6,4,7,8,1,9,5,2};
    int Size = size of (data) /size of (data[0]);
    bubblesort (data, size);
    printf ("Sorted array: ");
    for (i = 0; i< size ; i++){
        printf ("%d", data [i]);
    }
}


         OUTPUT 
4 6 7 1 8 5 9
4 6 1 7 5 8 9
4 1 6 5 7 8 9
1 4 5 6 7 8 9
1 4 5 6 7 8 9
1 4 5 6 7 8 9
sorted array: 1 4 5 6 7 8 9

Q(19) Implement selection sort:


             program 
#include <stdio.h>
    void selectionSort (int array[], int size){
    int step, i;
    for (step=0; step<size-1 ; step++){
    int min_idx= step;
    for (i= step+1 ; i<size ; i++){
    if(array[i] < array[min_idx]){
            min_idx = i;
    }
}
    int temp= array[min_idx];
    array[min_idx]= array[step];
    array[step]= temp;
      for (i=0; i<size; i++){
      printf("%d ", array[i]);
}
     printf("\n");
   }
}
    int main(){
    int i;
    int data []= {6,4,7,8,1,9,5};
    int size = size of (data)/size of (data [0]);
    SelectionSort (data, size);
    print f ("sorted array: ");
    for (i=0 ; i< size ; i++){
    print f ("%d", data [i]);
    }
}

               OUTPUT 
1      4      7      8      6      9      5
1      4      7      8      6      9      5
1      4      5      8      6      9      7
1      4      5      6      8      9      7
1      4      5      6      7      9      8
1      4      5      6      7      8      9

Sorted array : 1 4 5 6 7 8 9



Q(20) Implement Insertion sort


              PROGRAM 
# include < stdio.h>
   void insertion(int array [ ], int size){
   int i, step ;
   for (step = 1 ; step < size ; step++){
   int key = array [step];
   int j = step-1;
   while ( j>= 0 && key < array (j)){
   array [j+1] = array [j];
   --j;
}
   array [j+1] = key ;
       for (i=0; i < size ; i++ ){
       printf ("%d ", array [i]);
}
       printf ("\n");
   }
}
    int main() {
    int i;
    int data[] = { 6, 4, 7, 8, 1, 9,  5}
    int size = sizeof (data) / sizeof (data [0]);
    insertionSort (data, size);
    printf ("sorted array : ");
    for (i=0; i < size ; i++ ){
   printf ("%d ", data [i]);
  }
}
      
        OUTPUT 
4 6 7 8 1 9 5
4 6 7 8 1 9 5
4 6 7 8 1 9 5
1 4 6 7 8 9 5
1 4 6 7 8 9 5
1 4 5 6 7 8 9
sorted array : 1 4 5 6 7 8 9 


Q(21) modified bubble sort (Swap flag)


            PROGRAM 
#include <stdio.h>
    void bubblesort(int array[], int size){
    int step, i;
    int swap = 0;
    for (step = 0; step < size-1; step ++){
    for (i = 0; i < size-step-1; ++i){
       if (array[i] > array[i+1]){
       int temp = array[i];
       array[i] = array[i+1];
       array[i+1] = temp;
       swap ++ ;
   }
}
       if (swap == 0){
       break;
  }
        for(i = 0; i < size; i++){
            printf("%d", array[i]);
        }
          printf("\n");
    }
}
    int main(){
    int i;
    int data[] = {7, 5, 4, 8, 1};
    int size = size of (data) / size of (data[0]);
    bubblesort(data, size);
    printf("sorted array: ");
    for (i = 0; i < size; i++){
        printf("%d", data[i]);
    }
}


        OUTPUT 
5 4 7 1 8
4 5 1 7 8
4 1 5 7 8
1 4 5 7 8
Sorted array: 1 4 5 7 8


Q(22)Implement modified SelectionSort (min_idx & max_idx together)
   
   
          program 
#include <stdio.h>
     void SelectionSort (int array [], int size){
    int step, i;
    for (step = 0; step < size - 1 ; step++){
    int min_idx = step;
    for (i = step + 1 ; i < size ; i++){
    if (array [i] < array [min_idx]){
    min_idx = i;
   }
}
   int temp = array [min_idx];
   array [min_idx] = array [step];
   array [step] = temp;
   for (i = 0; i < size ; i++){
   printf ("%d ", array [i]);
}
   printf ("\n");
}
   for (step = size - 1 ; step > 0 ; step--){
   int max_idx = step;
   for (i = size - 1 ; i > step ; i--){
   if (array [i] > array [max_idx]){
   max_idx = i;
  }
}
int antemp = array[max_idx];
    array[max_idx] = array[size - 1];
    array[size - 1] = antemp;
    for (i = 0; i < size; i++) {
    printf("%d", array[i]);
}
    printf("\n");
}

   int main() {
   int i;
   int data[] = {6, 4, 7, 8, 1, 9, 5};
   int size = sizeof(data) / sizeof(data[0]);
   SelectionSort(data, size);
   printf("sorted array: ");
   for (i = 0; i < size; i++) {
   printf("%d", data[i]);
  }
}


           OUTPUT 
1 4 7 8 6 9 5
1 4 7 8 6 9 5
1 4 5 8 6 9 7
1 4 5 6 8 9 7
1 4 5 6 7 9 8
1 4 5 6 7 8 9
1 4 5 6 7 8 9
1 4 5 6 7 8 9
1 4 5 6 7 8 9
1 4 5 6 7 8 9
1 4 5 6 7 8 9
1 4 5 6 7 8 9
Sorted array: 1 4 5 6 7 8 9

        ASSIGNMENT: 6

Q.(23) Implement merge sort

         PROGRAM 
#include<stdio.h>
void merge (int arr[],int p,int q, int r){
  int n1 = q-p + 1;
  int n2 = r-q;
  int L[n1], M[n2];
  for(int i=0; i<n1; i++){
    L[i] = arr[p + i];
  }
  for (int j=0; j<n2; j++){
    M[j] = arr[q + 1 + j];
  }
  int i, j, k;
  i = 0;
  j = 0;
  k = p;
  while (i < n1 && j < n2){
    if (L[i] <= M[j]){
      arr[k] = L[i];
      i++;
    }
    else {
      arr[k] = M[j];
      j++;
    }
    k++;
  }
  while (i < n1){
    arr[k] = L[i];
    i++;
    k++;
  }
  while (j < n2) {
    arr[k] = m[j];
        j++;
        k++;
    }
}
void mergeSort(int arr[],int l, int r){
    if (l < r){
        int m = l + (r - l) / 2;
        mergeSort(arr, l, m);
        mergeSort(arr, m + 1, r);
        mergeSort(arr, l, m, r);
    }
}
int main() {
    int data[] = {4, 5, 7, 9, 1, 3, 8, 2, 6};
    int n = Size of (data) / Size of (data[0]);
    mergeSort (data, 0, n - 1);
    printf ("Sorted array: ");
    for (int i = 0; i < n; i++) {
        printf ("%d, ", data[i]);
    }
    return 0;
}



            OUTPUT 
sorted array: 1, 2, 3, 4, 5, 6, 7, 8, 9



Q(24) Implement Quick Sort

             program 
#include <stdio.h>
void swap (int array [], int a, int b) {
    int temp = array [a];
    array [a] = array [b];
    array [b] = temp;
}
    int partition (int array [], int low, int high) {
    int pivot = array[high];
    int i = low - 1;
    for (int j = low; j < high; j++) {
    if (array[j] <= pivot) {
        i++;
        swap(array, i, j);
    }
}
    swap(array, i + 1, high);
    return i + 1;
}
     void quicksort(int array[], int low, int high) {
     if (low < high) {
     int pi = partition(array, low, high);
      quicksort(array, low, pi - 1);
      quicksort(array, pi + 1, high);
    }
}
    int main() {
    int data[] = {4, 5, 7, 9, 11, 3, 8, 2, 6};
    quicksort(data, 0, 8);
    for (int i = 0; i < 9; i++) {
        printf("%d ", data[i]);
    }
    return 0;
}

             OUTPUT 
2 3 4 5 6 7 8 9 11


Q(25)Take an array of 10 element randomly unsorted Implement the sorting which checks two adjacent element and swap them if needed and perform the sorting for one external loop iteration. Then take that intermediate array passing to a sorting function which performs worst when array is sorted.


         PROGRAM 
#include <stdio.h>
    int Swap(int *x, int *y) {
    int temp = *x;
    *x = *y;
    *y = temp;
}
    int partition (int array [], int low, int high)
{
    int pivot = array [high];
    int i = low - 1;
    for (int j = low; j < high; j++)
{
    if (array [j] <= pivot)
{ i++;
    Swap(& array [i], & array [j]);
  }
}
    Swap(& array [i+1], & array [high]);
    return (i+1);
}
   void quicksort (int array [], int low, int high)
{
   if (low < high)
{
   int pi = partition (array, low, high);
quicksort (array, low, pi - 1);
quicksort (array, pi+1, high);
   }
}
    void bubble sort (int array [], int size)
{
    for (int step = 0; step < size - 1; step++)
  {
        int swap = 0;
        for (int i = 0; i < size - step - 1; ++i)
{
        if (array [i] > array [i+1])
{
        int temp = array [i];
        array [i] = array [i+1];
        array [i+1] = temp;
        swap = 1;
 }
      if (swap == 1)
    {
      quicksort (array , 0, size - 1);
            }
        }
    }
}
      int main ()
{
      int data [7] = { 6, 4, 7, 8, 1, 10, 5 };
      int size = size of (data) / size of (data [0]);
      bubble sort (data , size);
      Print f ("Sorted array : \n");
      for (int i = 0; i < size ; i + +)
{
        pintf (" % d", data [i]);
    }
}


           OUTPUT 
 Sorted array : 1 4 5 6 7 8 10




