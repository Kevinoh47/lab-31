![CF](http://i.imgur.com/7v5ASc8.png) LAB
=================================================

## Lab 31 Assignment 1 Connect to Store

### Author: Kevin O'Halloran

### Links and Resources
* [codesandbox for assignment 1](https://codesandbox.io/s/yq877nmj1x)

### Modules
#### `app.js`
App martials other components and renders the page for src/index.js.

##### Exported Values and Methods
src/components/app.js exports the App class. 

#### `changer.js`
The src/components/changer.js component builds out Change and Reset buttons for the fooReduxy component. 

##### Exported Values and Methods
It exports a react-redux connect function call for both mapStateToProps and mapDispatchToProps methods for the Changer class. These allow the class to pull state from the redux store.

#### `fooReduxy.js`
The src/components/fooReduxy functional component was created to replace the foo element on the page.

##### Exported Values and Methods
It exports a react-redux connect function call for the mapStateToProps method for the fooReduxy function. This allows the function to pull state from the redux store.

#### `name.js`
The src/components/name component is an implementation of a non-redux component which gets props from its parent component, app.js.

##### Exported Values and Methods
The Name functional component exports itself. App.js passes 

#### `nameReduxy.js`
The src/components/nameReduxy component was created to manage names via the redux store rather than the regular react parent-child architecture.

##### Exported Values and Methods
This functional component exports a react-redux connect function call for the mapStateToProps method for the function. This allows the function to pull state from the redux store.

#### `actions.js`
The src/store/actions.js defines the actions that will be taken when the redux store manages state changes for foo.

##### Exported Values and Methods
This exports changeFoo and resetFoo. changeFoo takes a payload for input. This will be the value that foo is expected to change to. resetFoo does not take a payload, since reset will always change foo back to the initalState.

#### `index.js`
The src/store/index.js is the main file for the redux store. It combines all individual reducers to manage state. (Usually this file defines a "reducers" object, but I have named this "state" to be more clear about what it is doing.)

##### Exported Values and Methods
This exports the createStore method for the combined reducers.

#### `person-reducer.js`
The src/store/person-reducer defines initial state for person name.

##### Exported Values and Methods
It exports a function that takes state and action as inputs, parses out the action into type and payload variables, and uses that information to define what will happen when a person's name is going to change or be reset.

#### `reducers.js`
The src/store/reducers.js file defines initial state for foo.

##### Exported Values and Methods
It exports a function that takes state and action as inputs, parses out the action into type and payload variables, and uses that information to define what will happen when foo is going to change or be reset.

#### `index.js`
scr/index is the main file for rendering the application. 

#### UML
![UML](./lab-31-assignment1-uml.jpg)
![UML](lab-31-assignment1-uml.jpg)
