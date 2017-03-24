# Sample_Java01
The purpose of this repository is to demonstrate basic knowledge in Java.

public class Demonstration {
public static void main(String[] args) {

/**
  This particular program will prompt users to enter their name, age, and location.
  Afterwards, the program will reiterate the user's input.
  If a valid age is not entered, an error message will be displayed and the user will have to input a valid number.
  NOTE: PROGRAM IS STILL IN THE WORKS. THERE MAY BE ERRORS.
*/

int age;
String input, name, location;

name = JOptionPane.showInputDialog("What is your name?");

input = JOptionPane.showInputDialog("What is your age?");

try {
age = Integer.parseInt(input);
    if (age < 0 || age > 115)
      {
       JOptionPane.showMessageDialog(null, "INVALID AGE. Enter an age between 0 and 115.");
      }
}

catch (NumberFormatException e) {
JOptionPane.showMessageDialog(null, "ERROR! Enter a valid age.");
}

location = JOptionPane.showInputDialog("In which country do you reside?");

JOptionPane.showMessageDialog(null, "Hello, " + name ".\nYou are currently " + age + " years old."
                              + "\nYou live in " + location.);
