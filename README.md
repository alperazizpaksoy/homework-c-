# homework-c-
C
#include <stdio.h>
#include <stdlib.h>
int main(int argc, char *argv[]) {
	int n, i, aranan, bulundumu = 0;
    printf("Dizinin kac elemanli olucagini giriniz: ");
    scanf("%d", &n);
    int dizi[n];
    printf("Dizinin elemanlarini giriniz: \n");
    for(i=0; i<n; i++) {
        scanf("%d", &dizi[i]);
    }
    printf("Aranacak elemani giriniz: ");
    scanf("%d", &aranan);
    for(i=0; i<n; i++) {
        if(dizi[i] == aranan) {
            printf("%d elemani dizinin %d. elemanidir.\n", aranan, i+1);
            bulundumu = 1;
            break;
        }
    }
    if(bulundumu == 0) {
        printf("%d elemani dizide bulunamadi.\n", aranan);
    }
	return 0;
}
