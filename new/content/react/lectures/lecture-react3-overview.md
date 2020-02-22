<!doctype html>
<html>
	<head>
    <title>React - Intro</title>
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

### 3. React</h3>
##### Overview</h5>

---


 #### React is a JavaScript library for building user interfaces.</h4>

---
        

#### React</h4>
          <ul>
            <li><a href="https://reactjs.org/">Documentation</a></li>
            <li><a href="https://github.com/facebook/react">Github</a></li>
            <li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">Reacts JavaScript level assumption</a></li>
          </ul>

---


#### React is Developed and maintained by Facebook (initial release 2013)</h4>
          <ul>
            <li>Apps built using React or React Native</li>
            <ul>
              <li>Facebook</li>
              <li>Netflix</li>
              <li>Instagram</li>
              <li>Dropbox</li>
              <li>WhatsApp</li>
              <li>Airbnb (styleguide, react-sketchapp)</li>
              <li>Wix (wix-style-react)</li>
            </ul>
          </ul>

---


#### Popular libraries in React projects</h4>
          <ul>
            <li><a href="https://reacttraining.com/react-router/web/guides/quick-start" target="_blank">react-router</a> - routing</li>
            <li><a href="https://redux.js.org/" target="_blank">redux</a> - State management</li>
            <li><a href="https://github.com/axios/axios" target="_blank">axios</a> - Promise based HTTP client</li>
            <li><a href="https://redux-form.com/8.1.0/" target="_blank">redux-form</a> - Handling forms with redux</li>
            <li><a href="https://github.com/reactjs/react-transition-group" target="_blank">react-transition-group</a> - Handling animations and transitions</li>
            <li><a href="https://github.com/css-modules/css-modules" target="_blank">CSS Modules</a> - Encapsulatied Styling (webpack)</li>
            <li><a href="https://github.com/styled-components/styled-components" target="_blank">styled-components</a> - JSS</li>
            <li><a href="https://github.com/airbnb/enzyme" target="_blank">Enzyme</a> - For additional testing utilities</li>
          </ul>

---


#### React</h4>
          <ul>
            <li>Design simple views for each state in your application, and React will efficiently update and render just the right components when your data changes.</li>
            <li>Build encapsulated components that manage their own state, then compose them to make complex UIs.</li>
            <li>Since component logic is written in JavaScript instead of templates, you can easily pass rich data through your app and keep state out of the DOM. - <a href="https://reactjs.org/">React-Documentation</a></p></li>
          </ul>

---


#### What is state?</h4>
          <ul>
            <li>The data that defines the condition of some object or system.</li>
            <li>Examples of states.</li>
            <ul>
              <li>The television is off.</li>
              <li>The coffee is hot.</li>
              <li>The clock is 14:15 am.</li>
            </ul>
            <li>Difference between a value and a variable</li>
            <ul>
              <li>The number 42 does not have a state since you can't change it.</li>
              <li>The number is a value</li>
            </ul>
          </ul>

---
        

#### Components</h4>
          <ul>
            <li>In React, every piece of a UI is a component.</li>
            <li>Components can be composed together to create other components.</li>
            <li>The application itself is a component, it's a composition of components.</li>
            <li>Every component is a Class (or function) that you can instantiate. That means that your component can receive arguments that you can use to customize what's shown in the application.</li>
          </ul>

---


####  Rendering output
* All React components have some kind of return or ```render()``` method.
* A component without a ```render()``` or return method is not a React component.
* The ```render()``` method returns a React element, which is its appearance.
* What it returns or renders is the output, a component must have an output.
* See this as a function, a component is something that returns an output based on input.


---


#### Virtual DOM</h4>
          <ul>
            <li>React uses a concept called Virtual DOM.</li>
            <li>This Virtual DOM is <b>NOT</b> the same as the ordinary DOM.</li>
            <li>For every DOM object, there is a corresponding “virtual DOM object, and this virtual DOM object is a representation of a DOM object, like a lightweight copy.</li>
          </ul>

---
        

#### Virtual DOM</h4>
          <ul>
            <li>The Virtual DOM selectively renders subtrees of nodes based upon state changes.</li>
            <li>It does the least amount of DOM manipulation possible in order to keep your components up to date.</li>
            <li>If there are any changes in the Virtual Dom then React performs a “diffing algorithm". Which identifies what has changed and accordingly updates the real DOM. This means that it doesn't update the entire DOM just the nodes that has changed.</li>
          </ul>

---


#### React compared to Angular</h4>
          <ul>
            <li>React is a JavaScript library while Angular is a complete Framework.</li>
            <li>React uses a Virtual DOM while Angular uses the regular DOM.</li>
            <li>React uses JSX while Angular uses plain HTML.</li>
            <li>React has one-way binding while Angular has two-way binding.</li>
            <li>React is more commonly used with JavaScript while Angular with TypeScript.</li>
            <li>React has a lower barrier when learning while Angular has a steep learning curve.</li>
          </ul>

---


#### A project created with create-react-app comes with:</h4>
          <ul>
            <li>React, JSX, ES6, TypeScript and Flow syntax support.</li>
            <li>Language extras beyond ES6 like the object spread operator.</li>
            <li>Autoprefixed CSS, so you don't need -webkit- or other prefixes.</li>
            <li>A fast interactive unit test runner with built-in support for coverage reporting.</li>
          </ul>

---


#### A project created with create-react-app comes with..</h4>
          <ul>
            <li>A live development server that warns about common mistakes.</li>
            <li>A build script to bundle JS, CSS, and images for production, with hashes and sourcemaps.</li>
            <li>An offline-first service worker and a web app manifest, meeting all the Progressive Web App criteria. (Note: Using the service worker is opt-in as of react-scripts@2.0.0 and higher)</li>
            <li>Hassle-free updates for the above tolis with a single dependency.</li>
          </ul>

---


#### A JavaScript build toolchain example</h4>
          <ul>
            <li>A package manager (Yarn, Npm)</li>
            <li>A bundler, (Webpack)</li>
            <li>A compiler (Babel)</li>
          </ul>

---


#### Creating an project</h4>
          <ul>
            <li>npx create-react-app my-app</li>

            <li>npx is an an NPM package runner</li>

            <li>You need to have atleast Node >= 6</li>
          </ul>

---


#### Create a new project with create-react-app and investigate it</h4>

---

