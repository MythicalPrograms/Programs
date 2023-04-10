Program to find the product of two 3x3 matrix
```c
#include <stdio.h>

int main() {
    
    int a[3][3], b[3][3], i, j, multi[3][3], sussy;
    
    printf("Enter the elements of matrix A:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("Enter the element a%d%d: ", i+1, j+1);
            scanf("%d", &a[i][j]);
        }
    }
    
    printf("\nEnter the elements of matrix B:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("Enter the element b%d%d: ", i+1, j+1);
            scanf("%d", &b[i][j]);
        }
    }
    
    printf("\nInput matrix A:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("%d\t", a[i][j]);
        }
        printf("\n");
    }
    
    printf("\nInput matrix B:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("%d\t", b[i][j]);
        }
        printf("\n");
    }
    
    printf("\nMultiplication of matrix A and B:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            multi[i][j] = 0;
            for (sussy = 0; sussy < 3; sussy++) {
                multi[i][j] = multi[i][j] + a[i][sussy] * b[sussy][j];
            }
        }
    }
    
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("%d\t", multi[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}```
