# Type Alias vs Interface in TypeScrip #
## Introduction: ##
In typescript Type Alis and Interface are two important features.Both are using to define structure and shap of data.Although they look like similar but the have some important differences.Now we will explore it using small code example.

We can create a new type using type keyword.This is called type alias. 
```typescript
type User = {
  name : string;
  email : string;
};

const user: User = {
  name : "Rahim",
  email : "rahim@gmail.com"
};
```
Here I create a type which name is User.It has two properties.
We can create a interface using interface keyword
```typescript
intrface User = {
  name : string;
  email : string;
};

const user: User = {
  name: "Rahim",
  email: "rahim@gmail.com"
};
```
Here I careate a interface which name is User. Both looks like same.But have some differences.Such as:
We can create Primitive Type using type.Like:
```
type name = string;
type Age = number;
type IsActive = boolean;
```
On the other hand inderface doesn't allow it.Like:
```
interface ID = string;
```
~~This is invalid.~~
We can create Union type using type but don't do it using interface. Like:
```
type User = "admin" | "user" | "manager"
const user : User = "user"
```
We can declare many interface as a same name.When it happens typescript automatically combine it.On the other hand type alias doesn't allow it.
```
interface User{
    name : string;
}
interface User{
    email : string;
}
const user : User = {
    name : "Akib",
    email : "xyz@gmail.com"
};
```
Here typescript merge two interface.
```
type User = {
    name : string;
}
```
### type User = .....Now it is invalid. ###
### Type Alias usecase ###
- Making primitive type
- Making union type
- Making intersection type
- Making tuple
- Making type composition
- Function type define

### Interface usecase ###
- Define structure if object
- Making class
- Making Mergining

## Conclusion

Both are important features of typescript.Type Alias is more flexible for complex types,on the otherhand Interface is useful for defining and extending object.
