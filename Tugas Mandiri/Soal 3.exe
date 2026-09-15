#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int compare(const void *a, const void *b) {
    int x = *(int *)a;
    int y = *(int *)b;

    if (x < y)
        return -1;
    else if (x > y)
        return 1;
    else
        return 0;
}

int main(void) {
    int N;

    scanf("%d", &N);

    int A[N];

    for (int i = 0; i < N; i++) {
        scanf("%d", &A[i]);
    }

    qsort(A, N, sizeof(int), compare);

    long long semua = (long long)N * (N - 1) / 2;
    long long sama = 0;

    int jumlah = 1;

    for (int i = 1; i < N; i++) {
        if (A[i] == A[i - 1]) {
            jumlah++;
        } else {
            sama += (long long)jumlah * (jumlah - 1) / 2;
            jumlah = 1;
        }
    }

    sama += (long long)jumlah * (jumlah - 1) / 2;

    long long kombinasi = semua - sama;

    printf("%lld\n", kombinasi);

    return 0;
}
