# Part 2: Authentication

For this assignment you will be adding to the previous part of this assignment

## Requirements
This assignment's main focus is adding google authentication via firebase.  Think of the login as being an administrator type login - when you log in you should see all dogs and all employees (just like before)

### Authentication
* Create a new firebase project
* Enable google authentication
* Move everything that was in App to the Home component - ie Home displays all dogs and employees
* Do everything we did in class on monday:
1. Have an Auth component with a login button
1. Clicking the login button should log your user in
1.  Create a navbar - when you are logged in you should see a brand and a logout button.  When you are logged out you should just see the brand,
1. Clicking the logout button in the navbar should log you out and return you to the auth screen

### Code specification
- All your code should be error free
- If you have a `this.props.SOMETHING` in a file you should have proptypes for that thing. If the SOMETHING is an object make a shape for it