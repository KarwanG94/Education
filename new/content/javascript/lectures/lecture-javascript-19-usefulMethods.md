
<!doctype html>
<html>
	<head>
    <title>JavaScript - Useful Methods</title>
    <meta charset="utf-8">
    <meta name="robots" content="noindex, nofollow">
		<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">

		<link rel="stylesheet" href="../../libs/reveal/css/reset.css">
		<link rel="stylesheet" href="../../libs/reveal/css/reveal.css">
		<link rel="stylesheet" href="../../libs/reveal/css/theme/softhouse.css">

		<link rel="stylesheet" href="../../libs/bootstrap/css/bootstrap.min.css">
		<link rel="stylesheet" href="../../style.css">

		<script src="../../libs/jquery/jquery.min.js"></script>
		<script src="../../libs/bootstrap/js/bootstrap.min.js"></script>


		<!-- Theme used for syntax highlighting of code -->
		<link rel="stylesheet" href="../../libs/reveal/lib/css/monokai.css">
	</head>
	<body>
		<nav class="navbar navbar-expand-lg  navbar-dark bg-dark fixed-top shadow-lg">
			<a class="navbar-brand" href="https://www.softhouse.se">
				<?xml version="1.0" encoding="utf-8"?>
				<!-- Generator: Adobe Illustrator 22.1.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
				<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
					viewBox="0 0 928 179" style="enable-background:new 0 0 928 179;" xml:space="preserve">
				<style type="text/css">
					.st0{fill:#FFFFFF;}
				</style>
				<g>
					<path class="st0" d="M795,121.4c-9.5,4.3-6.3,24.8-15.8,31.6c-5.3,3.8-31,4-34.3-3.8c-4.7-11.1,30.2-28.8,23.5-38.9
						c-8.6-12.9-58.5-8.8-61.6-18c-1-3.1,7-17.5,17.7-18.8c11.8-1.9,31.6,19.9,48.2,19.4c32.2-1.1,34.9-51.8,58.5-58
						c20.7-5.4,37.6-1.6,38.8,7.3c2.2,17.3-59.7,45.1-55.8,59.8c4.9,18.6,74.6,26.4,73.8,41.5c-0.4,7.2-13.7,12.5-25.1,9.6
						C840.6,147.4,818.1,111,795,121.4 M866.5,166.7c20.8,6.4,53.4,1.7,54.2-13.4c1.5-30.6-93.3-36.1-99.1-53
						c-3.8-11.2,85.4-49.2,83.1-73.3c-1.4-15.1-33.7-18-62.2-12.1C787.6,26,807.3,84,772.8,86.7c-14.9,1.2-32.8-26.1-54.2-26.1
						c-13.9,0-33,25.6-30.3,33.2c5.8,16.9,63.6,6.4,73.2,20.1c5.8,8.2-36,26.9-27.8,45.2c4.6,10.2,40.9,14.6,52.1,5
						c9.3-7.9,4.9-34.5,12.1-37.7C814.7,119,839.5,158.4,866.5,166.7"/>
					<path class="st0" d="M62.8,101.3H21.3v9.8h30.5c9.3,0,12.2,2.2,12.2,11v6.4c0,8.7-2.9,11-12.2,11H11v-8.7h42.7l0-10.7H23.3
						c-9.2,0-12.3-2.2-12.3-11v-5.1c0-8.8,3.1-11,12.3-11h39.4V101.3z"/>
					<path class="st0" d="M571.8,101.3h-41.4v9.8h30.5c9.3,0,12.2,2.2,12.2,11v6.4c0,8.7-2.9,11-12.2,11H520v-8.7h42.7v-10.7h-30.4
						c-9.2,0-12.3-2.2-12.3-11v-5.1c0-8.8,3.1-11,12.3-11h39.4V101.3z"/>
					<path class="st0" d="M81.5,103.9v24.5c0,8.8,2.9,11,12.2,11H130c9.2,0,12.2-2.2,12.2-11v-24.5c0-8.9-3-11-12.2-11H93.7
						C84.5,92.9,81.5,95,81.5,103.9 M93,101.5h37.9v29H93V101.5z"/>
				</g>
				<polygon class="st0" points="159.8,92.9 209.3,92.9 209.3,101.3 171.3,101.3 171.3,113.4 197.2,113.4 197.2,122.1 171.3,122.1
					171.3,139.5 159.8,139.5 "/>
				<polygon class="st0" points="256.5,139.5 245.1,139.5 245.1,101.3 222.6,101.3 222.6,92.9 279.3,92.9 279.3,101.3 256.5,101.3 "/>
				<polygon class="st0" points="292.5,92.9 304,92.9 304,110.6 339.7,110.6 339.7,92.9 351.2,92.9 351.2,139.5 339.7,139.5
					339.7,119.9 304,119.9 304,139.5 292.5,139.5 "/>
				<g>
					<path class="st0" d="M368.6,103.9v24.5c0,8.8,2.9,11,12.2,11h36.3c9.2,0,12.2-2.2,12.2-11v-24.5c0-8.9-3-11-12.2-11h-36.3
						C371.6,92.9,368.6,95,368.6,103.9 M380.1,101.5h37.8v29h-37.8V101.5z"/>
					<path class="st0" d="M458.3,130.8H491V92.9h11.5v35.5c0,8.7-3,11-12.3,11h-31.1c-9.3,0-12.2-2.3-12.2-11V92.9h11.4V130.8z"/>
				</g>
				<polygon class="st0" points="590.5,92.9 640.9,92.9 640.9,101.2 602.1,101.2 602.1,111.3 627.1,111.3 627.1,119.4 602.1,119.4
					602.1,130.8 641.5,130.8 641.5,139.5 590.5,139.5 "/>
				</svg>
			</a>
			<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
				<span class="navbar-toggler-icon"></span>
			</button>

			<div class="collapse navbar-collapse" id="navbarSupportedContent">
				<ul class="navbar-nav m-auto">
					<script src="../../navigation.js"></script>
				</ul>
			</div>
    </nav>
    
		<div class="reveal">
			<div class="slides">

### 19. JavaScript</h3>
##### Useful methods</h5>

---
        

#### Built in methods</h4>
          <ul>
            <li>In this lecture we will look into built the built in methods:</li>
            <ul>
              <li>Iterating over them extracting values.</li>
              <li>Filtering out values.</li>
              <li>Sorting values.</li>
              <li>Converting objects into arrays.</li>
              <li>Creating new arrays from other arrays.</li>
            </ul>
          </ul>

---


#### Arrays and Objects</h4>
          <ul>
            <li>Handling objects and arrays is something developers do on a daily basis.</li>
            <ul>
              <li>Array.map()</li>
              <li>Array.filter()</li>
              <li>Object.keys()</li>
              <li>Object.values()</li>
              <li>Object.entries()</li>
            </ul>
          </ul>

---


### But first the classic For loop</h3>

---


####  Iterating over Arrays with for loop

            ```JavaScript
            let array1 = [1, 4, 9, 16];
            let newArray = [];

            for(let i = 0; i < array1.length; i++){
                let newValue = array1[i] * 2;
                newArray.push(newValue);
            }
            
            console.log(newArray); // [2, 8, 18, 32]
            ```


---


####  For...of loop

* The for...of statement creates a loop iterating over iterable objects, including: built-in String, Array, array-like objects (e.g., arguments or NodeList), TypedArray, Map, Set

            ```JavaScript            
            const array1 = ['a', 'b', 'c'];

            for (const element of array1) {
              console.log(element);
            }
            ```
            <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...of">MDN reference</a>


---


          #### Iterating over Objects with For
          
          * The for...in statement iterates over all non-Symbol, enumerable properties of an object.

          ```JavaScript
          let string1 = "";
          let object1 = {a: 1, b: 2, c: 3};
          
          for (let property1 in object1) {
            string1 += object1[property1];
          }
          
          console.log(string1); "123"
          ```

          [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in)


---


####  Array.map()

* The map() method creates a new array with the results of calling a provided function on every element in the calling array.
            
            ```JavaScript
            let array1 = [1, 4, 9, 16];

            // pass a function to map
            const map1 = array1.map(function(x){
             return x * 2
            } );

            console.log(array1); // still [1, 4, 9, 16] since a new Array was created.
            console.log(map1); // [2, 8, 18, 32]
            ```
            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)


---


####  Array.filter()

* The filter() method creates a new array with all elements that pass the test implemented by the provided function.
            
            ```JavaScript
            let words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

            const result = words.filter(function(word){
              return word.length > 6
            });
            
            console.log(words); // still ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'] since a new Array was created.
            console.log(result); // ["exuberant", "destruction", "present"]
            
            ```
            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)


---


####  Object.keys()

* The Object.keys() method returns an array of a given object's own enumerable property names, in the same order as we get with a normal loop.
            
            ```JavaScript
            const object1 = {
              a: 'somestring',
              b: 42,
              c: false
            };
            
            console.log(Object.keys(object1)); // ["a", "b", "c"]
            
            ```
            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)


---


####  Object.values()

* The Object.values() method returns an **array** of a given object's own enumerable property values, in the same order as that provided by a for...in loop.

            ```JavaScript
            const object1 = {
              a: 'somestring',
              b: 42,
              c: false
            };
            
            console.log(Object.values(object1)); // ["somestring", 42, false]
            
            ```
            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/values)


---


####  Object.entries()

* The Object.entries() method returns an array of a given object's own enumerable string-keyed property [key, value] pairs, in the same order as that provided by a for...in loop             
            
            ```JavaScript
            const object1 = {
              a: 'somestring',
              b: 42,
              c: false
            };
            
            console.log(Object.entries(object1)); // [ ["a", "somestring"], Array ["b", 42], Array ["c", false]]
            
            ```
            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/entries)


---


#### Other good to know methods.</h4>

---


####  Array.every()

* The every() method tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value. 
            
            ```JavaScript
            let array = [1, 2, 3, 4, 5];

            let even = function(element) {
              // checks whether an element is even
              return element % 2 === 0;
            };
            
            console.log(array.every(even)); // expected output: false
            ```
            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/some)


---


####  Array.some()

*  The some() method tests whether at least one element in the array passes the test implemented by the provided function. It returns a Boolean value.

            ```JavaScript
            function isBelowThreshold(currentValue) {
              return currentValue < 40;
            }

            let array1 = [1, 30, 39, 29, 10, 13];

            console.log(array1.some(isBelowThreshold)); // expected output: false
            ```
            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/every)


---


####  Array.sort()

* The sort() method sorts the elements of an array
            
            ```JavaScript
            let months = ['March', 'Jan', 'Feb', 'Dec'];
            months.sort();
            console.log(months);
            // expected output: Array ["Dec", "Feb", "Jan", "March"]
            
            let array1 = [1, 30, 4, 21, 100000];
            array1.sort();
            console.log(array1);
            // expected output: Array [1, 100000, 21, 30, 4]
            ```

            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)


---


####  Array.concat()

* The concat() method is used to merge two or more arrays. This method does not change the existing arrays, but instead returns a new array.  
            
            ```JavaScript
            let array1 = ['a', 'b', 'c'];
            let array2 = ['d', 'e', 'f'];
            
            console.log(array1.concat(array2)); // expected output: Array ["a", "b", "c", "d", "e", "f"]
            ```
            [MDN reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/concat)


---


### <a href="https://github.com/SofthouseVxo/Education" target="_blank">Github examples!</a></h3>

---
