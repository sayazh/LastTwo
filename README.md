# LastTwo
String exercise
package stringAssignments;

import java.util.Scanner;

public class LastTwo {
	public static void main(String[] args) {

		Scanner scan = new Scanner(System.in);

		System.out.println("Enter please any word");
		String word = scan.next();
		char ch1 = word.charAt(word.length() - 1);
		char ch2 = word.charAt(word.length() - 2);
		String change1 = word.replace(ch2, ch1);

		if (word.length() >= 2) {
			System.out.println(change1.substring(0, change1.length() - 1) + ch2);
		} else {
			System.out.println("Valid word");
		}
		scan.close();
	}
}
