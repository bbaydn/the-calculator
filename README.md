//the-calculator
// First project with C
//The calculator says hi to user in Turkish


#include<stdio.h>
#include <stdlib.h>
#include<math.h>

int main()
{
	
	int islem;
	int a,b;
	int sonuc;
	char name[20];
	
	printf("Isminiz nedir?\n");
	fgets(name, 20, stdin);
	printf("Merhaba %s su anda bbaydn tarafindan yapilan ilk hesap makinesi ile konusuyorsun. \n", name);
	
	printf("Yapmak istedigin islemi sayi ile gosterir misin? \n 1- Toplama\n 2- Cikarma\n 3- Carpma\n 4- Bolme\n 5- Us alma\n 6- Karekok\n");
	scanf("%d", &islem);
	

	if (islem==1){
		printf("%s Ilk sayiyiyi yazar misin?\n", name);
		scanf("%d",&a);
	
		printf("%s Ikinci sayiyi yazar misin\n", name);
		scanf("%d",&b);

	
		sonuc= a + b;
		printf("Sonuc= %d", sonuc);
}
	else if (islem==2)	{
		printf("%s Ilk sayiyiyi yazar misin?\n", name);
		scanf("%d",&a);
	
		printf("%s Ikinci sayiyiyi yazar misin?\n", name);
		scanf("%d",&b);
		
		sonuc= a - b;
		printf("Sonuc= %d", sonuc);
}
	else if(islem==3){
		printf("%s Ilk sayiyiyi yazar misin?\n", name);
		scanf("%d",&a);
	
		printf("%s Ikinci sayiyiyi yazar misin?\n", name);
		scanf("%d",&b);
		
		sonuc= a*b;
		printf("Sonuc= %d", sonuc);
}
	else if(islem==4){
		printf("%s Ilk sayiyiyi yazar misin?\n", name);
		scanf("%d",&a);
	
		printf("%s Ikinci sayiyiyi yazar misin?\n", name);
		scanf("%d",&b);
		
		sonuc= a/b;
		printf("Sonuc= %d", sonuc);
} 
	else if(islem==5){
		printf("%s Ilk sayiyiyi yazar misin?\n", name);
		scanf("%d",&a);
	
		printf("%s Ikinci sayiyiyi yazar misin?\n", name);
		scanf("%d",&b);
		
		sonuc= pow(a,b);
		printf("Sonuc= %d", sonuc);
}
	else if(islem==6){
		printf("%s Kok islemi yapmak istedigin sayiyiyi yazar misin?\n", name);
		scanf("%d",&a);
		sonuc =sqrt(a);
		printf("Sonuc= %d", sonuc);
	}
	else
		printf("%s Hatali giris yaptin. Programi yeniden baslatmalisin.", name);
	
	return 0;		
}
