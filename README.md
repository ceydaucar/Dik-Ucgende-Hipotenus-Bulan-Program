# Dik Üçgende Hipotenüs Bulan Program
Patika.dev > Java101 > Pratik3 - Dik Üçgende Hipotenüs Bulan Program

## Üç kenar uzunluğunu kullanıcıdan aldığınız üçgenin alanını hesaplayan programı yazınız.
### Formül
- Üç𝑔𝑒𝑛𝑖𝑛 ç𝑒𝑣𝑟𝑒𝑠𝑖 = 2𝑢
- 𝑢 = (a+b+c) / 2
- Alan * Alan = 𝑢 * (𝑢 − 𝑎)* (𝑢 − 𝑏) * (𝑢 − 𝑐)
	
		import java.util.*;
		
		public class pratik3 {
		
			public static void main(String[] args) {
		
				// Yeni bir tarayıcı(scanner) oluştur.
				Scanner sc = new Scanner(System.in);
		
				//Kullanıcıdan uzunluk değerlerini al.
				System.out.println("Kenar uzunluklarını girin: ");
				int a = sc.nextInt();
				int b = sc.nextInt();
				int c = sc.nextInt();
		
				// Formülleri uygula.
				int u = (a + b + c) / 2;
				int cevre = 2 * u;
				double alan = Math.pow(u*(u-a)*(u-b)*(u-c), 0.5);
		
				// Sonucu yazdır.
				System.out.println("Alan: " + alan);
			}
		}
