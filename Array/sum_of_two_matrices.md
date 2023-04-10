Program to read any 2x2 matrix and display in format.
```c
#include <stdio.h>
int main() {
    
    int a[3][3], b[3][3], i, j, sum[3][3];
    
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("Enter the element of matrix A: ");
            scanf("%d", &a[i][j]);
        }
    }
    
    printf("\n");
    
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("Enter the element of matrix B: ");
            scanf("%d", &b[i][j]);
        }
    }
    
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            sum[i][j] = a[i][j] + b[i][j];
        }
    }
    
    printf("\nSum of Matrix A and B:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("%d\t", sum[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}
```
