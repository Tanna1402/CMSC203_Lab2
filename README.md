# CMSC203_Lab2
import java.util.Scanner;
public class SphereVolume {

	public static void main(String[] args) {
		// Add your declaration and code here
		Scanner input = new Scanner(System.in);
		String purpose = "This program will calculates the volume of a sphere using the diameter given my user and predefined math function.";
		System.out.println(purpose);
		System.out.print("\n");
		System.out.println("Please enter the diameter of the sphere: ");
		double diam = input.nextDouble();
		if (diam>0) {
			double radius;
			final double num = 2;
			radius = diam/num;
			double vol;
			vol = (4/(double)3)*Math.PI*(Math.pow(radius, 3));
			System.out.println("The volume of the sphere is " + vol + " unit square.");
		}
		else {
			String error = "Diameter must be greater than 0." + "\nPlease try again!";
			System.out.println(error);
		}
	}

}
