
import java.util.*;
public class pratik1 {

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
