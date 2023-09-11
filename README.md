#include <stdio.h>

int main() {
    int n, i;
    printf("Give a number: ");
    scanf("%d", &n);

    if (n <= 1) {
        printf("Not prime\n");
        return 0;
    }

    for (i = 2; i < n; i++) {
        if (n % i == 0) {
            printf("Not prime\n");
            return 0;
        }
    }

    printf("Prime\n");
    return 0;
}
