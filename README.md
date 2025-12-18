# ppcm
ppcmm
#include <stdio.h>

int ppcm(int a, int b) {
    int max = (a > b) ? a : b;
    while (1) {
        if (max % a == 0 && max % b == 0)
            return max;
        max++;
    }
}

int main() {
    int x, y;
    printf("Entrez le premier nombre: ");
    scanf("%d", &x);
    printf("Entrez le deuxieme nombre: ");
    scanf("%d", &y);
    printf("Le PPCM de %d et %d est %d\n", x, y, ppcm(x, y));
    return 0;
}
