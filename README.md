# srm-web-designing-using-react-js
Info about web designing using react js
# WEB DESIGN INTERN
## DAY-1
* installation of Git tool and Github account and new repository
## Day-2
* Repository editss
* md : mark down syntax for documentation*
* cloning into local systems*
* creating folders and files in local system folders and pushing them into github repository*
## DAY-3
* Sublime text editor installation
* INTRO TO HTML5 (tags,its elements types,images(logos)insertion)
* Editing index file using tags and forms.
## DAY-4
* DIFFERENT TYPES of elements in Html5
  ** block line elements
  ** IN line elements
  **  navigation elements
  ** ssemantic ..
 * CSS
## DAY-5
### FLex properties : These are the advanced concepts of css grid system
 * display: flex;
	 * flex-direction : row-reverse;
	 * flex-wrap: wrap;
	 * justify-content: center;
##DAY-6
### Profile creation  : (using flex properties)
        * profile with name , profession 
	* mail ,tel navigations & other communication details along with their link address.
	
## DAY-7
* Bootstrap dwnld... and remaining css properties

## DAY-8
### About Bootstrap.mim.css &  Bootstrap.mim.js
    * bootstrap clases 
    * txt colors, bg colors , btns , grid system
    
## DAY-9
 * table & its properties using bootstrap
 
 ## DAY-10
 * Intro to js and data types
 ## DAY-11
 * alert("hi")
undefined
* prompt("enter")
"JIM"
* confirm("Are u sure")
false
* Console statements
* functions
* Array iterations using Map() , for in , for of .
## DAY-12
### DOM of js : document functions , documenty selectors.
* We can implement JavaScript code any where in html document.
* We've to use script tags for taht (<script> </script>)
* By using document keyword, We can manipulate the data in html document.
* Document object model functions are:
  * document.getElementById("id");
* Collections :
  * document.getElementsByClassName("className");
  * document.getElementsByTagName("Tag name");
* Common statements for DOM
  * document.querySelector("#selector | .selector | Tag Name Selector");
  * document.querySelectorAll(".selector | Tag Name Selector");


## DAY-13
## innerHTML :
  * innerHTML triggers the information exist with in the tags.
     * Example:
  ```javascript
	* <div id ="second">
		Sample division
	</div>
	var second=document.getElementById("second").innerHTML;
	console.log(second);
	____
	Output: Sample division
 ```
* Writing information into divisions using innerHTML

	document.getElementById("second").innerHTML="Hello everyone";
* Creating and appending HTML attributes We can create the html attributes by using javascript code part also. For that we need to use document.createElement. And we can append the information into the created elements by using textContent.

Syntax:

	document.createElement("html tagname")
Example:

	//Selecting a section from html;
	var secondDiv=document.getElementById("second");
	
	// Creating a html attribute
	var heading2=document.createElement("h2");
	heading2.textContent="heading";
	
	//Appending child attribute to parent
	secondDiv.appendChild(heading2);
## Objects in Javascript
* Object is nothing but its a key,value pair. When we going to get the value from an object, we've to use the key of that object

Example:
```javascript

	var student={
		name:"Hemanth sai",
		role:"Student",
		branch:"CSE:
	}
	__________
	student.name => Hemanth sai
	
```
## Arrays in the object:
```javascript

	var student={
		friends:["sai vasanth","savya sree", "nitesh bharti","venkatesh"]
	}
	_____
	// Here `0` is the index value
	student.friends[0]
	______
	Output: sai vasanth
	
	_____
	student.friends[student.friends.length-1]
	____
	Output: Venkatesh
```
## Objects in Object:
 ```javascript

	var student={
		student1:{
			name:"Swetha"
		},
		student2:{
			name:"venkatesh"
		}
	}
	______
	student.student1.name
	_____
	Output: Swetha
 ```
	
# DAY-14

## Java Script Object Notation(JSON)
* Light weight data-interchange format (This is a format to trnsfer information between the nodes)
* This is very easy to read,understand and write.
* This is very easy for the machines to parse and generate data.
* This is subset of javascript programming language standards (ECMA SCRIPT - 262).
* For accessing JSON data from a HTML document, we need to use a server.
     * npm server
     * web server for chrome (200 OK)
          Web server for chrome is a static server invented google team. This allows us to access any information from               external file into a HTML document.
     * Installation of 200 OK
            * Type web server for chrome in your chrome browser and press Enter.
            *  We have to choose web server for chrome from chrome.google.com from listing.
            *  We have to click on add to chrome button. Soon after we will see a dialogue box and then click on add app.
## Promises:
* A promise is an object that may produce a single value some time in the future. The client and the server communicating with eachother, client need to send a request to the server, the server need to respond to the client request simultaniously. This promise give us a value that the is resolved or not resolved. The states for the promise are

* Fulfilled
* Rejected
* Pending
 * The promise is a chine relation, We can build multiple coding blocks. The syntax:
 ```javascript

	promise(request).then(response=>{
		return response;
	})
 ```
* Promises examples:

* Fetch
* Cache
 * Example:
     
     ```javascript
     
	fetch('data.json').then(response=>{
		return response.json();
	}).then(data=>{
		console.log(data);
	})
     ```
* The promioses concept is the replacement for XMLHttpRequest. The XMLHttpRequest provides a way to communicate with client and server
# DAY-15
* Code practice on json, promises.


## React
### Features of React
* Its a library
* Virtual DOM : _Its enable us to build scalable and fast applications_.
* JSX
* Components
	* Functional Components (Stateless component)
	* Class Component (Statefull component)
	* Pure components
	* Higher Order Components (HOC's)
* One way data binding

### States and props in React
**S**tate provides an ability to store information in the components. With in class component only we can use the state concept. We've to use the constructor method as well as the super method for initializing the state as we need information from the base class. By using `this.state` we can initialize a state. The state should be in object format. 

Syntax:
```javascript
	constructor(){
    		super();
    		this.state={
      		name:"Hanuman"
    		}
  	}
```

We can implement the state concept in class component only.

#### But how we are going to implement the state functionality in a functional component ?
We can implement this by using the concepts called **Hooks**.
**H**ooks are new feature introduced in React 16.8 version. It allows us to use states and other React features without writing the class. We can implement the hooks in functional components.

Example:
	**useState**
	This is for implementing the states concept in functional components.
	
Syntax
```javascript
	// Importing useState functionality from the base class
	import React,{useState} from 'react';

	let StatesInFunction=()=>{
		// Here count is for initializing the value and setCount is for manipulating the initialized value
    		const [count,setCount]=useState("Bye");
    		return(
        		<div>
				<h2 
					onMouseOver={()=>setCount("Hi")}
					onMouseLeave={()=>setCount("Bye")}> {count} 
				</h2>
        		</div>
    			)
		}

	export default StatesInFunction;
```


Example II :
```javascript
	import React,{useState} from 'react';

	let StatesInFunction=()=>{
    		let initialValue=0;
    		let [count,setCount]=useState(initialValue);
    		return(
        	  <div>
            		<h2> {count} </h2>
            		<button onClick={()=>{setCount(count-=-1)}}> Increment </button>
            		<button onClick={()=>{setCount(count-=1)}}> Decrement </button>
            		<button onClick={()=>{setCount(count=initialValue)}}> Initial </button>
        	  </div>
    		)
	}

	export default StatesInFunction;
```

### Props in React
+ **P**rops is a special keyword in React which is used for passing the data from one component to another component.
+ It is uni-directional
+ props data is read-only, which means the data coming from the parent component should not be changed by child components.
+ Props are arguments passed among React components.

Example: (Passing properties (`props`) from class component to a functional component)
App.js
```javascript
	import React,{Component} from 'react';
	import './App.css';
	import StatesInFunction from './StatesInFunction';
	
	class App extends Component{
  	
	render(){
        return (
    		<div className="App"> 
			// Props	
      			<StatesInFunction name="Nitesh" age="20 years"/>

    		</div>
    		)
  	   }
	}


export default App;
```
StatesInFunction.js
```javascript
	import React from 'react';

	let StatesInFunction=(props)=>{
    		return(
        		<div>
            			<h2> {props.name} is {props.age} </h2>
            			<h2> {count} </h2>
        		</div>
    		)
	}

	export default StatesInFunction;
```
#### But how we are going to access the props in class components
Here we go with that
```javascript
	import React from 'react';

	export default class StatesInFunction extends React.Component{
    		render(){
        		return(
            			<div>
                			<h2> {this.props.name} is {this.props.age} old. </h2>
            			</div>
        		)
    		}
	}
```
### Routing in React (react-router-dom)
`npm install react-router-dom --save`

#### Primary components of React-route-dom:
* BrowserRouter
	
	Is usefull for initializing the navigation context. This is the parent component of `react-router-dom`
	
```javascript
		<BrowserRouter>
		</BrowserRoputer>
```
* Route
	
	Is for specifying the path.
	
```javascript
		<Route exact path="/about" component={About}>
		</Route>
```

```javascript
		<BrowserRouter>
			<Route exact path="/about" component={About} />
		</BrowserRouter>
```
* Link

	This is for providing event that calls to the path specified in the path of route component.
	
```javascript
		<Link to="/about"> Click me </Link>
		// <a href="/about"> Click me </a>
```

Example:

```javascript
	<BrowserRouter>
		<Route path="/about" component={About}/> 
	<BrowserRouter>
	
	<Link to="/about" />
```

Most of the web developers or web designers uses the link attribute (`<a> </a>`) to pass the data from one page to another page.

In react we are using the `<Link> </Link>` attribute instead of anchor tag (`<a> </a>`).

#### But how we are going to pass data from one component to another component using `<Link />` ?

For this we have to pass the parameters in the format of object as shown below.

```javascript
	<Link to={{pathname:"/resume", data:{id:index}}} className="button"> View profile </Link>
```

* Here the `pathname` specifies the url we are going to navigate.
* `data` represents the information which we are passing. Here `id` is the key and the `index` is the value.

If you wanna access that information in destination component, we've to use the `location` keyword.

```javascript
	import React from 'react';
	import {profiles} from './data.json';
	import './App.css';

	let Resume=(props)=>{
    	var info=profiles[props.location.data.id];
    	return(
        	<section className="parent"> 
            		<article className="basicsCard"> 
                		<h2> {info.basics.name} </h2>
            		</article>
        	</section>
    		)
	}

	export default Resume;
```

## Node JS
### node with mysql
Installing mysql

`npm install mysql`

#### COnnecting with mysql

```javascript
	var mysql = require('mysql');

	// mysql connection
	var connection=mysql.createConnection({
		host:"localhost",
		user:"root",
		password:""
	});
	
	connection.connect(err=>{
		if err throw err
		console.log("Connected to mysql");
	})
```

#### Creating a database
```javascript
	connection.connect(err=>{
	if (err) throw err;
	console.log("Connected to mysql");
	connection.query("CREATE DATABASE node-info", (err,result)=>{
		if(err) throw err;
		console.log(result);
		})
	})
```

#### Creating a table
```javascript
	var connection=mysql.createConnection({
		host:"localhost",
		user:"root",
		password:"",
		**database**:"node_info"
	});

	connection.connect(err=>{
		if (err) throw err;
		console.log("Connected to mysql");
		connection.query("CREATE TABLE employee (name varchar(20), emaild varchar(50), mobile varchar(20))",(err,result)=>{
			if(err) throw err;
			console.log("Table created");
		})
	})
```

#### Inserting Data
```javascript
	connection.connect(err=>{
	if (err) throw err;
	console.log("Connected to mysql");
	connection.query("INSERT INTO employee (name,emaild,mobile) VALUES ('Hemanth','hemanth@gmail.com','9888786858')",(err,result)=>{
		if(err) throw err;
		console.log("Table created");
		})
	})
```

