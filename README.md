# Problem-Solving-Project
###Find the Missing Number
#include <stdio.h>

int main() {
    int T;
    scanf("%d", &T);

    for(int i = 0; i < T; i++) {
        long long M, A, B, C;
        scanf("%lld %lld %lld %lld", &M, &A, &B, &C);

        long long product = A * B * C;

        if(product == 0) {
            if(M == 0)
                printf("0\n");
            else
                printf("-1\n");
        }
        else {
            if(M % product == 0)
                printf("%lld\n", M / product);
            else
                printf("-1\n");
        }
    }

    return 0;
}
