Program to find transpose of a 2x3 matrix and display them
```c
#include <stdio.h>
int main() {
    
    int a[2][3], transpose[3][2], i, j;
    
    printf("Enter the elements of matrix:\n");
    for (i = 0; i < 2; i++) {
        for (j = 0; j < 3; j++) {
            printf("Enter the element of matrix a%d%d: ", i + 1, j + 1);
            scanf("%d", &a[i][j]);
        }
    }
    
    printf("\nInput Matrix:\n");
    for (i = 0; i < 2; i++) {
        for (j = 0; j < 3; j++) {
            printf("%d\t", a[i][j]);
        }
        printf("\n");
    }
    
    for (i = 0; i < 2; i++) {
        for (j = 0; j < 3; j++) {
            transpose[j][i] = a[i][j];
        }
    }
    
    printf("\nTranspose of input matrix:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 2; j++) {
            printf("%d\t", transpose[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}
```
