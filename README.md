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


    
