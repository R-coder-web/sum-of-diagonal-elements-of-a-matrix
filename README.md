# sum-of-diagonal-elements-of-a-matrix
#include <stdio.h>
int main(){
int a[10][10],i,j,n,row,col,sum=0;
printf("enter the row and column of a matrix: ");
scanf("%d %d",&row,&col);
printf("\n");
for(i=0;i<row;i++){
printf("\n");
for(j=0;j<col;j++){
printf("a[%d][%d]: ",i,j);
scanf("%d",&a[i][j]);
}
}
printf("\n");
printf("Matrix A: ");
for(i=0;i<row;i++){
printf("\n");
printf("\t");
for(j=0;j<col;j++){
printf("%d ",a[i][j]);
}
}
printf("\n");
for(i=0;i<row;i++){
for(j=0;j<col;j++){
if(i==j){   //condition for diagonal elements:
printf("%d ",a[i][j]);      //print the diagonal elements:
sum=sum+a[i][j];        //calculate the sum of diagonal elements:
}
}
}
printf("\n");
printf("sum of diagonal elements are %d: ",sum);
}
