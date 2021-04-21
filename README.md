# BTVN
Bài tập về nhà buổi 1

import java.util.Scanner;

public class BaiTapVeNha1234 {

	public static void main(String[] args) {
		BaiTapVeNha1234.PhuongTrinhBacHai();
		BaiTapVeNha1234.findMaxInArray();
		BaiTapVeNha1234.showDayOfMonth();
		BaiTapVeNha1234.replaceString();
	}

	public static void PhuongTrinhBacHai() {
		System.out.println("Bai tap 1: Tinh phuong trinh bac 2: Moi nhap tham so a, b, c:");
		float a, b, c;
		Scanner nhapSo = new Scanner(System.in);
		a = nhapSo.nextFloat();
		System.out.println("Gia tri a =" + a);
		b = nhapSo.nextFloat();
		System.out.println("Gia tri b =" + b);
		c = nhapSo.nextFloat();
		System.out.println("Gia tri c =" + c);
		if (a != 0) {
			float delta = (-b) * (-b) - 4 * a * c;
			System.out.println("Gia tri delta =" + delta);
			if (delta > 0) {
				float x1, x2;
				x1 = (float) ((-b + Math.sqrt(delta)) / 2 * a);
				x2 = (float) ((-b - Math.sqrt(delta)) / 2 * a);
				System.out.println("Phuong trinh co 2 nghiem la:" + "x1 = " + x1 + "\n" + "x2 =" + x2);
			} else if (delta == 0) {
				float x;
				x = -b / a;
				System.out.println("Phuong trinh co nghiem kep la =" + x);
			} else if (delta < 0) {
				System.out.println("Phuong trinh vo nghiem");
			}
		} else if (a == 0) {
			float x3;
			x3 = -b / a;
			System.out.println("Phuong trinh co 2 nghiem la =" + x3);
		}
	}

	public static void findMaxInArray() {
		System.out.println("Bai tap 2: Lay phan tu lon nhat trong mang 101 phan tu tu 0 den 100:");
		int a[] = new int[] { 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24,
				25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50,
				51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76,
				77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100 };
		int max = a[0];
		for (int i = 0; i < a.length; i++) {
			if (a[i] > max) {
				max = a[i];
			}
		}
		System.out.println("Max la: " + max);
	}

	public static void showDayOfMonth() {
		System.out.println("Bai tap 3: Dua ra so ngay cua 1 thang trong nam, moi nhap thang:");
		Scanner thang = new Scanner(System.in);
		Scanner nam = new Scanner(System.in);
		int a = thang.nextInt();
		System.out.println("Thang ban nhap la:" + a);
		if (a < 1 || a > 12) {
			System.out.println("Khong ton tai thang nay");
		} else {
			switch (a) {
			case 1, 3, 5, 7, 8, 10, 12:
				System.out.println("Thang " + a + "co 31 ngay.");
				break;
			case 4, 6, 9, 11:
				System.out.println("Thang " + a + "co 30 ngay.");
				break;
			case 2:
				System.out.println("Ban nhap thang 2, ban phai nhap them nam: ");
				int b = nam.nextInt();
				System.out.println("Ban nhap nam: " + b);
				if (b % 4 == 0) {
					System.out.println("Ban nhap thang " + a + " nam " + b + " la nam nhuan!");
					System.out.println("Thang 2 nam " + b + " co 29 ngay!");
				} else {
					System.out.println("Thang 2 " + b + " co 28 ngày!");
				}

			}
		}
	}

	public static void replaceString() {
		System.out.println("Bai tap 4: Replace chuoi:");
		String s1 = "Tôi tên là Nguyen Tran Trung. Tôi đang là Auto Tester1";
		String s2 = "Le Thi Hong";
		String s3 = "Automation Tester";
		String replaceString = s1.replace("Nguyen Tran Trung", s2);
		String replaceString1 = replaceString.replace("Auto Tester1", s3);
		System.out.println(replaceString1);
	}

}

Bài 5:


public class Employee {
	String ID, Name;
	int Age;
	float Salary;
	public static void main(String[] args) {
		
	}
	public void Employee() {
		this.ID = ID;
		this.Name = Name;
		this.Age = Age;
		this.Salary = Salary;
	}
	
	public String getID() {
		return ID;
	}
	
	public String Name() {
		return Name;
	}
	
	public int Age() {
		return Age;
	}
	public float Salary() {
		return Salary;
	}

}

