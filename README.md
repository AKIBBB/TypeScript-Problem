# Overview #
## First Problem: ##
This function has two parameter.One perameter value is required and other one multiplier is optional.Thats why I use optional perameter multiplier(`?`) If multiplier is undefiend then the function return value * 2.Otherwise it returns value * multiplier.
## Second Problem ##
This problem is based on Union type and Type Narrowing.This function accecpts varoius type input like (`String`) (`Number`) and (`Boolean`).That means value takes string, number or boolean.Then I find the type of value using (`typeof`).
If the value is string then trim the whitespace using (`trim()`) function and then make the string in lowercase using (`toLocaleLowerCase()`) function.
If the value is number then multiply it by 10.
If the value is boolean then I check the value is true or false.If value is true fuction  return "Active".If value is false then return "Inactive".

## Third Problem ##
This is Array Destructing and Tuple Type problem.I use tuple and `Readonly Modifier`.Topule has three value.Firts value type is number,second value type is number and third value type is string.For using Readonly, cant't change the touple value.Then distructure the array.Finally return the output using template literal for desire return format.

## Fourth Problem ##
This problem based on Generics. `T` is a generic type.This fuction accepts various type array.According to input typescript itself determine the type.`...` Using rest perameter I take multiple array.Every array type is `T`.The using `flat()` function to make it a single array.

## Fifth Problem ##
First create a `Interface` name course.I make `interface` to create a object.Then declare a function name `getPopularCourses`.`Course take multiple object and find the minimum number of students.If course is published and cousrse.student >= minstudents then return the object.

## Sixth Problem ##
This problem based on generics.Here I use two geceric type `T and K`.`T` find the data type of object and `K` find the data type of property.This function takes input as a array of object.`Keyof` find the all key of objct.`K extends Keyof T` It prevents the use of any key that doesnt't exist in object.I use map to find the property value of object and make new array which conatains property value.Finally return the array.

## Seventh Problem ##
It is a class based problem.Here Employee is the parent class and Manager is the child class.Manager class ingerit the Employee class.First make a parent class Employee.In this class name is `protected` and baseSalary is `private`.So name is accessable in child class but baseSalary is only accessable in Employee class.Then make a consructor for Employee.Employee class has one method which returns Employee name and baseSalary.
Manager class extends Employee.So Manager class inherit Employee class proprties and method.Manger class has private property department and then make a constructor for Manager class.Use `super` for calling parent class constructor so that access the private property of Employee class.Manager class has one method which return name and department.Finally create a object call the function.`manager.getDetails()` how can I call it? Because Manager inherit Employee.

## Eighth Problem ##
This is a `Asyncronous` function.It takes a age as a input.Fuction returns a promise which is string type.I make a new promise.If promise is succseeds then call `resolve` otherwise `reject`.If age is lower than 18 promise is rejected and call a `new Error()` for making error instance.Here is no delay.
If age is higher than 18`setTimeout()` is executed.After one second `resolve()` will be executed.I call the function using `await`.Because await waits for the result of promise.I use top level await thats why I export
```
export {};
```
## Blog 1 ##
[Type vs Interface](./type-interface-1.md)
## Blog 2 ##
[Union Intersection Types](./union-intersection-types-2.md)
