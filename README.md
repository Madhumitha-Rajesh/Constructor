# Constructor

Coding-

package constructor;
import java.util.Scanner;
class Person {
    String name;
    int age;
    public Person() {
        this.name = "Madhumitha";  
        this.age = 18;           
    }
    public Person(String name, int age) {
        this.name = name;  
        this.age = age; 
    }
    public void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

public class Constructor {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Person person1 = new Person();
        person1.displayInfo();  
        System.out.println();
        System.out.print("Enter name for the second person: ");
        String name = scanner.nextLine();  

        System.out.print("Enter age for the second person: ");
        int age = scanner.nextInt(); 
        Person person2 = new Person(name, age); 
        scanner.close();
    }
}


Output-

Name: Sakthi
Age: 18

Enter name for the second person: Vivek
Enter age for the second person: 18
