-class Employee
{
        String name;
        int id;
        int sal;
        public Employee(String name, int id, int sal)
        {
                this.name = name;
                this.id = id;
                this.sal = sal;
        }
        public void getDetails()
        {
                System.out.println("Name: " + name);
                System.out.println("Employee No.: " + id);
                System.out.println("Salary: " + sal);
        }
}
class Manager extends Employee
{
        String dept;
        public Manager(String name, int id, int sal, String dept)
        {
                super(name, id, sal);
                this.dept = dept;
        }
        public void getDetails()
        {
                super.getDetails();
                System.out.println("Department: " + dept);
        }
}
public class cl2
{
        public static void main(String [] args)
        {
        Employee emp = new Employee("Joe Mama", 101, 69000);
        emp.getDetails();
        System.out.println();
        Manager mg = new Manager("Sugma", 102, 420000, "Sales");
        mg.getDetails();
        }
}
                
