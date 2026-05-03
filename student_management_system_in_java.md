# 🎓 Student Management System in Java

Ye Java ka bohat popular beginner-to-intermediate level project hai jo almost har Java learner OOP aur Collections seekhne ke baad banata hai.

Is project me:

* Classes
* Objects
* ArrayList
* Loops
* Methods
* Encapsulation
* User Input
* CRUD Operations

sab use hote hain.

---

# 🚀 Features

✅ Add Student
✅ View Students
✅ Search Student
✅ Delete Student
✅ Simple Console Based UI

---

# ☕ Java Code

```java
import java.util.ArrayList;
import java.util.Scanner;

class Student {

    private int id;
    private String name;
    private double marks;

    public Student(int id, String name, double marks) {
        this.id = id;
        this.name = name;
        this.marks = marks;
    }

    public int getId() {
        return id;
    }

    public String getName() {
        return name;
    }

    public double getMarks() {
        return marks;
    }

    @Override
    public String toString() {
        return "ID: " + id +
               ", Name: " + name +
               ", Marks: " + marks;
    }
}

public class StudentManagementSystem {

    public static void main(String[] args) {

        ArrayList<Student> students = new ArrayList<>();
        Scanner sc = new Scanner(System.in);

        while (true) {

            System.out.println("\n===== Student Management System =====");
            System.out.println("1. Add Student");
            System.out.println("2. View Students");
            System.out.println("3. Search Student");
            System.out.println("4. Delete Student");
            System.out.println("5. Exit");

            System.out.print("Enter Choice: ");
            int choice = sc.nextInt();

            switch (choice) {

                case 1:

                    System.out.print("Enter ID: ");
                    int id = sc.nextInt();
                    sc.nextLine();

                    System.out.print("Enter Name: ");
                    String name = sc.nextLine();

                    System.out.print("Enter Marks: ");
                    double marks = sc.nextDouble();

                    students.add(new Student(id, name, marks));

                    System.out.println("Student Added Successfully!");
                    break;

                case 2:

                    if (students.isEmpty()) {
                        System.out.println("No Students Found!");
                    } else {

                        System.out.println("\nStudents List:");

                        for (Student s : students) {
                            System.out.println(s);
                        }
                    }

                    break;

                case 3:

                    System.out.print("Enter Student ID to Search: ");
                    int searchId = sc.nextInt();

                    boolean found = false;

                    for (Student s : students) {

                        if (s.getId() == searchId) {

                            System.out.println("Student Found:");
                            System.out.println(s);

                            found = true;
                            break;
                        }
                    }

                    if (!found) {
                        System.out.println("Student Not Found!");
                    }

                    break;

                case 4:

                    System.out.print("Enter Student ID to Delete: ");
                    int deleteId = sc.nextInt();

                    boolean removed = students.removeIf(s -> s.getId() == deleteId);

                    if (removed) {
                        System.out.println("Student Deleted Successfully!");
                    } else {
                        System.out.println("Student Not Found!");
                    }

                    break;

                case 5:

                    System.out.println("Exiting Program...");
                    sc.close();
                    System.exit(0);

                default:
                    System.out.println("Invalid Choice!");
            }
        }
    }
}
```

---

# 🧠 Concepts Used

| Concept        | Usage                  |
| -------------- | ---------------------- |
| Class & Object | Student class          |
| Encapsulation  | Private variables      |
| Constructor    | Student initialization |
| ArrayList      | Store students         |
| Loops          | Display/search         |
| Switch Case    | Menu handling          |
| Methods        | Getters & toString     |
| OOP            | Complete structure     |

---

# 📌 Future Improvements

You can upgrade this project using:

* File Handling
* Database (MySQL)
* GUI (Java Swing / JavaFX)
* Login System
* Attendance System
* Grade Calculation

---

# ⭐ Perfect For

* GitHub Portfolio
* Java Practice
* College Projects
* OOP Revision
* Interview Preparation
