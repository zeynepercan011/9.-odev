# odev9

/*kullan�c�dan pozitif bir tam say� de�eri alan ve bu say�n�n ka� basamakl� oldu�unu ekranda g�steren program. basamak_bul() isimli fonksiyon kullan�ls�n
ve hem de�er als�n hem de�eri d�nd�rs�n*/

#include<stdio.h>
int basamak_bul(int);
int main(void)
{
	int x;
	printf("bir tam sayi giriniz.");
	scanf("%d" , &x);
	
	printf("basamak sayisi: %d" , basamak_bul(x));
	
	return 0;
}

int basamak_bul(int x)
{
	int toplam=0;
	while(x>0){
		x=x/10;
		toplam++;
	
	}
	
	return toplam;
	
}
