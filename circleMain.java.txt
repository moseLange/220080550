package za.ac.wsu.driver.s220080550;

import za.ac.wsu.s220080550.Circle;

public class CircleMain {
	public static void main(String[] args) {
		// creates 3 Circle objects
		Circle c1 = new Circle();
		Circle c2 = new Circle();
		Circle c3 = new Circle();
		
		// set values to circle objects
		c1.setRadius(10);
		c1.setX(3);
		c1.setY(6);
		
		c2.setRadius(5);
		c2.setX(10);
		c2.setY(15);
		
		c3.setRadius(7);
		c3.setX(14);
		c3.setY(17);
		
		// displays the information of these circles
		System.out.println("Circle 1 Information");
		displayInformation(c1);
		System.out.println("\nCircle 2 Information");
		displayInformation(c2);
		System.out.println("\nCircle 3 Information");
		displayInformation(c3);
	}
	
	/**
	 * Displays information of circle
	 * @param c
	 */
	public static void displayInformation(Circle c) {
		System.out.println("Radius: "+c.getRadius() +", Center: (" +c.getX() + ", " + c.getY() +")");
		System.out.printf("Area: %.2f",c.calculateArea());
		System.out.printf("\nCircumference: %.2f",c.calculateCircumference());
		System.out.printf("\nDiameter: %.2f",c.calculateDiameter());
		System.out.println();
	}
}