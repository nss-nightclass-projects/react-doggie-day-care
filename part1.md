# Part 1: Basic state and props
For this assignment you will be building up a doggie day care using what you know about state and props with basic React.

## Requirements
For this project we will be building out the main two sections of the DOM - the dogs and the employees.

### Dogs
- A file `src/helpers/data/dogsData.js` should have an array called dogs filled with dog objects (see ERD)
- dogsData should export a function called `getAllDogs` that returns the dogs array
- The DogPen component should import the Dog component
- App should call `dogsData.getAllDogs()` to get the dogs array and pass the array of dogs into `DogPen.printDogs`

- `DogPen.printDogs` should map over the array passed into it and call the Dog component, passing in an individual dog each time.
- The Dog component should display the dog in a way of your choosing.

### Employees
- A file `src/helpers/data/employeesData.js` should have an array called employees filled with employee objects (see ERD)
- employeesData should export a function called `getAllEmployees` that returns the employees array
- The StaffRoom component should import the Employee component
- App should call `employeesData.getAllEmployees()` to get the employees array and pass the array of employees into `StaffRoom.printEmployees`
- `StaffRoom.printEmployees` should map over the array passed into it and call the Employee component, passing in an individual employee each time.
- The Employee component should display the employee in a way of your choosing.

### Code specification
- All your code should be error free
- If you have a `this.props.SOMETHING` in a file you should have proptypes for that thing. If the SOMETHING is an object make a shape for it