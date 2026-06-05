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

                            Magical tree
          
#include <stdio.h>

int main() {
    int N;
    scanf("%d", &N);

    int width = N + 10;

  
    for(int i = 1; i <= width; i += 2) {

        int space = (width - i) / 2;

        for(int j = 0; j < space; j++) {
            printf(" ");
        }

        for(int j = 0; j < i; j++) {
            printf("*");
        }

        printf("\n");
    }


    for(int i = 0; i < 5; i++) {

        int space = (width - N) / 2;

        for(int j = 0; j < space; j++) {
            printf(" ");
        }

        for(int j = 0; j < N; j++) {
            printf("*");
        }

        printf("\n");
    }

    return 0;
}
