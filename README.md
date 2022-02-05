#include <stdio.h>
#include <stdlib.h>
#include <ctype.h>
void bul_harf_buyukucuk(char x[]);
 int main(){
      char metin[100];
     printf("Metin giriniz:");
     gets(metin);
     bul_harf_buyukucuk(metin);
     return 0;}
void bul_harf_buyukucuk(char x[]){
 int sayac=0,kSayac=0,bSayac=0;
 while(x[sayac] != '\0')
 {
 if(islower(x[sayac])){
 kSayac++;}
 else if(isupper(x[sayac])){
 bSayac++;}
 sayac++;}
 int toplam=kSayac+bSayac;
 printf("Girilen metin icerisinde %d kucuk %d buyuk harf,toplam %d harf bulunur.", kSayac,bSayac,toplam);
 }
