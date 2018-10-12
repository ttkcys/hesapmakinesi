#include<stdio.h>
#include<math.h>
#include<conio.h>

void toplama (void);
void cikarma (void);
void carpma (void);
void bolme (void);
void karesi (void);
void karekok (void);
int main(void);

int main() 
{
	int islem;
	
	printf("1) Toplama\n"); 
	printf("2) Cikarma\n"); 
	printf("3) Carpma\n"); 
	printf("4) Bolme\n"); 
	printf("5) Karesi\n"); 
	printf("6) Karekok\n");
	printf("Yapmak istediginiz islem numarasını seciniz: ");
	scanf("%d",&islem);
	
	switch (islem)
	{
		case 1: toplama(); break;
		case 2: cikarma(); break;
		case 3: carpma(); break;
		case 4: bolme(); break;
		case 5: karesi(); break;
		case 6: karekok(); break;
		
		default : printf("Bu sayfaya aktarılmıs islem yoktur!!!");
				break;
			
		
	}
	return 0;	
}

	void toplama (void)
	{
		int sayi1,sayi2,toplam,kontrol;
		printf("sayi1 gir: ");
		scanf("%d",&sayi1);
		
		printf("sayi2 gir: ");
		scanf("%d",&sayi2);
		
		toplam=sayi1+sayi2;
		printf("sonuc=%d\n",toplam);
		
		printf("baska islem yapmak icin lutfen 1 e basın yoksa 0 a basın");
		scanf("%d",&kontrol);
		if (kontrol==1) main();
		
		return;
	}
	
		void cikarma (void)
	{
		int sayi1,sayi2,cikarma,kontrol;
		printf("sayi1 gir: ");
		scanf("%d",&sayi1);
		
		printf("sayi2 gir: ");
		scanf("%d",&sayi2);
		
		cikarma=sayi1-sayi2;
		printf("sonuc=%d\n",cikarma);
		
		printf("baska islem yapmak icin lutfen 1 e basın yoksa 0 a basın");
		scanf("%d",&kontrol);
		if (kontrol==1) main();
		
		return;
	}
	
		void carpma (void)
	{
		int sayi1,sayi2,carpma,kontrol;
		printf("sayi1 gir: ");
		scanf("%d",&sayi1);
		
		printf("sayi2 gir: ");
		scanf("%d",&sayi2);
		
		carpma=sayi1*sayi2;
		printf("sonuc=%d\n",carpma);
		
		printf("baska islem yapmak icin lutfen 1 e basın yoksa 0 a basın");
		scanf("%d",&kontrol);
		if (kontrol==1) main();
		
		return;
	}
	
		void bolme (void)
	{
		int sayi1,sayi2,kontrol;
		float bolme;
		
		printf("sayi1 gir: ");
		scanf("%d",&sayi1);
		
		printf("sayi2 gir: ");
		scanf("%d",&sayi2);
		
		bolme=sayi1/sayi2;
		printf("sonuc=%.2f\n",bolme);
		
		printf("baska islem yapmak icin lutfen 1 e basın yoksa 0 a basın");
		scanf("%d",&kontrol);
		if (kontrol==1) main();
		
		return;
	}
	
		void karesi (void)
	{
		int sayi1,kare,kontrol;
		printf("karesini almak istediğiniz sayıyı girin: ");
		scanf("%d",&sayi1);
		kare=pow(sayi1,2);
		
		printf("%d sayisinin karesi %d dir\n",sayi1,kare);
		
		printf("baska islem yapmak icin lutfen 1 e basın yoksa 0 a basın");
		scanf("%d",&kontrol);
		if (kontrol==1) main();
		
		return;
	}
	
	
		void karekok (void)
	{
		int sayi1,kontrol;
		float karekok;
		
		printf("karekokunu bulmak istediğiniz sayıyıgiriniz: ");
		scanf("%d",&sayi1);
		
		karekok=sqrt(sayi1);
		
		printf("%d sayısının karekoku %.2f dir\n",sayi1,karekok);
		
	
		printf("baska islem yapmak icin lutfen 1 e basın yoksa 0 a basın");
		scanf("%d",&kontrol);
		if (kontrol==1) main();
		
		return;
	}
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
