#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main(void) {
int A, B, C;
int kecil, tengah, besar;
int akhir;

scanf("%d %d %d", &A, &B, &C);

if (A <= B && A <= C) {
    kecil = A;
} else if (B <= A && B <= C) {
    kecil = B;       
} else {
    kecil = C;
} 
if (A >= B && A >= C) {
    besar = A;
} else if (B >= A && B >= C) {
    besar = B;
} else {
    besar = C;
}
tengah = A + B + C - kecil - besar;

if (tengah - kecil < besar - tengah) {
    akhir = tengah - kecil;
} else {
    akhir = besar - tengah;
}

printf("%d\n", akhir);

    return 0;
}