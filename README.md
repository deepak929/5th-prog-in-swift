# 5th-prog-in-swift
init and destuctor in swift
import UIKit

class Employee{
    var eid:Int?
    var ename:String?
    var salary:Double?
    //Default constructor
    init()
    {
    eid = 0
        ename = String()
    salary = 0.0
    }
    //Parametrize Constuctor
    init(employeeId eid:Int, employeeName
    ename:String,employeeSalary salary:Double)
    {
    self.eid = eid
    self.ename = ename
    self.salary = salary
    }
    init(emp:Employee)
    {
        self.eid = eid
        self.ename = ename
        self.salary = salary
        
    }
    func display()
    {
        print(self.eid!,self.ename!,self.salary!)
    
    }
    //Destructor
    deinit {
        print("Employee object Destroyed")
    }
}
var e1 = Employee()
//Employee.display(e1)
//print(e1,eid!, e1.name!, e1.salary!)
e1.display()
var e2 = Employee(employeeid: 1, employeename:"DEEEPAK SINGAM", employeesalary: 5000.0)
e2.display()
e1 = e2
e2 = e1
var e3 = e2
e3.display()


var e4 = Employee(emp: e1)
e4.ename = "SAGAR"
e4.display()


 e3.display()
 
 var e5 = e3
e5.ename=kareema"
e5.display()

e3.display()
/*
var eid = Int()
var gender = Bool()
var enm = String()
var salary = Double()
print(eid, gender, enm, salary)
 */
