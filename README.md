package comunityuni.com;

import java.util.Scanner;

public class HinhChuNhat {
	Scanner scanner = new Scanner(System.in);
	private double Chieu_dai , Chieu_rong; 
	
	//Khoi tạo costructor
	public HinhChuNhat(double Chieu_dai, double Chieu_rong)
	{
		this.Chieu_dai = Chieu_dai; 
		this.Chieu_rong = Chieu_rong; 
	}
	
	public HinhChuNhat() 
	{}
	//Khoi tao getter va setter
	public double getCd()
	{
		return Chieu_dai;
	}
	public void setCd() {
		this.Chieu_dai = Chieu_dai; 
	}
	
	public double getCr()
	{
		return Chieu_rong;
	}
	public void setCr() {
		this.Chieu_rong = Chieu_rong; 
	}
	//Khoi tao constructor nhap vao cdai, crong
		public void nhap()
		{
			System.out.println("Nhap chieu dai: ");
			Chieu_dai = scanner.nextDouble();
			System.out.println("Nhap chieu rong: ");
			Chieu_rong = scanner.nextDouble();
		}
	
	double TinhChuVi() {
		
		return (Chieu_dai + Chieu_rong) * 2;
	}
	
	double TinhDienTich()
	{
		return Chieu_dai * Chieu_rong;
	}
}
