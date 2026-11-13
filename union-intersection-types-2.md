# Practical Example of Combining Union (`|`) and Intersection (`&`) Types in TypeScript

## Introduction ##
In Typescript Union (`|`) and Intersection (`&`) type can combine to create a new flexible and reusable type.Using union (`|`) we can assign multiple type in a single variable.Using intersection (`&`) we can combine multiple type in a single type.Now we explore it using a example.

```
type User = {
    id : number;
    name : string;
};
type Admin = {
    role : "admin";
    permission : string[];
}
type Customer = {
    role : "customer";
    cart : string[];
};
type PlatformUser = User & (Asmin | Customer);

const admin : PlatformUser ={
    id : 1,
    name : "ABC",
    role : "admin",
    permission : ["create", "delete", "edit"]
};

const customer :  PlatformUser ={
    id : 1,
    name : "ABC",
    role : "customer",
    cart : ["T-shirt", "Pant", "Polo-Shirt"]
};
```
## Conclusion ##
In this example a user must have common properties of (`User`) and must also have either (`Admin`) or (`Customer`) type.So this is vry usefull to create complex data structure.