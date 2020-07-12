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
		``` document.getElementById("id");
* Collections :
		* document.getElementsByClassName("className");
		 * document.getElementsByTagName("Tag name");
* Common statements for DOM
		* document.querySelector("#selector | .selector | Tag Name Selector");
		* document.querySelectorAll(".selector | Tag Name Selector");


## DAY-13
## innerHTML :
  * innerHTML triggers the information exist with in the tags. Example:

	<div id="second">
		Sample division
	</div>
	var second=document.getElementById("second").innerHTML;
	console.log(second);
	____
	Output: Sample division
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

	var student={
		name:"Hemanth sai",
		role:"Student",
		branch:"CSE:
	}
	__________
	student.name => Hemanth sai
## Arrays in the object:

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
## Objects in Object:

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

	promise(request).then(response=>{
		return response;
	})
* Promises examples:

* Fetch
* Cache
 * Example:

	fetch('data.json').then(response=>{
		return response.json();
	}).then(data=>{
		console.log(data);
	})
* The promioses concept is the replacement for XMLHttpRequest. The XMLHttpRequest provides a way to communicate with client and server
# DAY-15
* Code practice on json, promises.

