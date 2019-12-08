# Part 3: Basic CRUD

For this assignment you will be adding to the previous part of this assignment.

## Requirements
Now that you got authentication working its time to assign some employees to walk some dogs.  We will be creating a new firebase collection called walks and performing full crud on that collection.

### Doggy and Employee Data
Currently you have a dogsData.js file and an employeesData.js file.  These both contain an array of objects.  Lets put that information into firebase.
* create `db/base.json` seed file.  this should have the following code:
```
{
  "dogs": 'moo',
  "employees": 'moo',
  "walks": 'moo'
}
```
* Create `db/dogs.json` seed file with the information that was in dogs.js - no arrays.  You will need to modify this data so it looks like normal firebase data - object of objects.
* Create `db/employees.json` seed file with the information that was in employees.js - no arrays.  You will need to modify this data so it looks like normal firebase data - object of objects.
* Create `db/walks.json` seed file and add some dummy data.  Each walk should look something like this:
```
{
  "walk1": {
    "dogId": "dog2"
    "employeeId": "employee4"
    "date": "10/25/2019"
  }
}
```
* Import all these seed files into firebase
* Create `axios.get` calls for dogs and employees so you are once again displaying all dogs and all employees on the Home page.

### CREATE Walks
* Create a form somewhere on your Home component that allows you to select a dog name from a dropdown, an employee name from a dropdown, and type in a date to an input (set the type='date').
* Once you click a save button on the form you should see a new walk in firebase

### READ Walks
* Display all walks saved in firebase.  Your display should show the dog name, employee name, and day they are getting walked.

### UPDATE Walks
* Have some kind of button on the walk that when you click it pre-populates a form like you used in CREATE so you can edit the walk.

### DELETE Walks
* Have some kind of button on that walk that when you click the it the walk is deleted from firebase and no longer displays on the app.

### Authentication
* When the user is logged out you should only be able to see the authentication page
* When the user is logged in you should be able to see everything but the authentication page.

### Code specification
- All your code should be error free
- If you have a `this.props.SOMETHING` in a file you should have proptypes for that thing. If the SOMETHING is an object make a shape for it
