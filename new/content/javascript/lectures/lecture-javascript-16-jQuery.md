<!doctype html>
<html>
	<head>
		<title>JavaScript - jQuery</title>
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

### 16. JavaScript</h3>
##### jQuery a JavaScript Library</h5>

---


#### What is jQuery?</h4>

---


#### According to jQuery themselves</h4>
					<p>
            jQuery is a fast, small, and feature-rich JavaScript library. It makes things like <b>HTML document traversal</b> and <b>manipulation</b>, <b>event handling</b>, <b>animation</b>, and <b>Ajax</b> much simpler with an easy-to-use API that works across a multitude of browsers. 
            With a combination of versatility and extensibility, jQuery has changed the way that millions of people write JavaScript. - <a href="https://jquery.com/">jQuery.com</a>
          </p>

---
        

#### JQuery according to w3schools</h4>
          <ul>
            <li>jQuery is a lightweight, "write less, do more", JavaScript library.</li>
            <li>The purpose of jQuery is to make it much easier to use JavaScript on your website.</li>
            <li>jQuery takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code.</li>
            <li>Simplifies a lot of the complicated things from JavaScript, like AJAX calls and DOM manipulation.</li>
          </ul>

---


#### jQuery doesn't do anything you cannot achieve with pure JavaScript.</h4>

---


####  Example
            Changes the HTML in the button element with the class 'continue' to 'Next Step...'

            ```JavaScript
            $("button.continue").html("Next Step...");
            ```
            How would you do this with vanilla JS?


---


####  Downloading jQuery

* <a href="https://jquery.com/download/" target="_blank">Downloads</a>
* <a href="https://code.jquery.com/">CDN's</a>
* npm ```npm install jquery --save```



---


#### jQuery source code</h4>

					<img style="margin-top: 0px;" src="/new/media/javascript-images/javascript-16/jquery.png" alt="jquery source code">

---


####  Inspect jQuery
            
* Include jQuery in your project and ```console.log(window)``` and locate jQuery in the object.
* **$** is simply an alias for jQuery and it's often employed because it's shorter and faster to write.

            ```JavaScript
            console.log(window.jQuery); // jQuery function
            console.log(window.$); // jQuery function same as above
            console.log(jQuery); // jQuery function same as above
            console.log($); // jQuery function same as above
            console.log(typeof $) // function
            ```


---


####  The jQuery function

* jQuery is exposed as a function.
* jQuery functions returns an object, and this can have properties and methods which it has.

            ```JavaScript
            // The jQuery method lets you find one or more elements on a page.
            $('button').addClass('primary-button') // { 0: button.primary-button, 1: button.primary-button }
            ```

            ```JavaScript
            console.log(jQuery('button.primary-button')); 
            ```


---


#### Basic syntax is: $(selector).action() </h4>
          <ul>
            <li>A $ sign to define/access jQuery</li>
            <li>A (selector) to "query (or find)" HTML elements</li>
            <li>A jQuery action() to be performed on the element(s)</li>
          </ul>

---


          #### Basic syntax - selectors

          * jQuery uses CSS syntax to select elements.

          ```JavaScript
          $("p").hide() // hides all <p> elements.

          $(".test").hide() // hides all elements with class="test".

          $("#test").hide() // hides the element with id="test".
          ```
          [More examples of jQuery selectors](https://www.w3schools.com/jquery/jquery_selectors.asp)


---


          #### jQuery event methods

          * In jQuery, most DOM events have an equivalent jQuery method.
          * Event methods trigger or attach a function to an event handler for the selected elements.
          
          jQuery
          ```JavaScript
          $("#my-button").click(function(){
            // code...
          }); 
          ```

          Vanilla JS
          ```JavaScript
          let myButton = document.getElementById('my-button');
          myButton.addEventListener("click", function() {
            // code...
          });
          ```
          [List of jQuery event methods](https://www.w3schools.com/jquery/jquery_ref_events.asp)


---


          #### Document ready function
    
          * Code included inside $( document ).ready() will only run once the page DOM is ready for code to execute.
          
          jQuery
          ```JavaScript
          $(document).ready(function(){
            $("p").click(function(){
              $(this).hide();
            });
          });
          ```

          Vanilla JS
          ```JavaScript
          document.addEventListener("DOMContentLoaded", function() {
            // code...
          });
          ```


---


          #### jQuery effects
    
          * **hide & show** 
          * toggle
          * animate
          
          jQuery
          ```JavaScript
          $("#hide").click(function(){
            $("p").hide();
          });
          
          $("#show").click(function(){
            $("p").show();
          }); 
          ```


---


          #### jQuery effects
    
          * **hide & show** 
          * toggle
          * animate
          
          jQuery
          ```JavaScript
          $("#hide").click(function(){
            $("p").hide(1000); // takes 1s to hide
          });
          
          $("#show").click(function(){
            $("p").show(1000, function(){  // Callback called when fully visible again after 1s.
              console.log('fully visible'); 
            });
          }); 
          ```
          [Try on w3schools](https://www.w3schools.com/jquery/tryit.asp?filename=tryjquery_hide_show)


---


          #### jQuery effects - toggle
    
          * toggles between hidden and shown
          
          jQuery
          ```JavaScript
          $("button").click(function(){
            $("p").toggle();
          }); 
          ```
          [Try on w3schools](https://www.w3schools.com/jquery/tryit.asp?filename=tryjquery_toggle)


---


          #### jQuery effects - animate
  
          ```JavaScript
          //  $(selector).animate({params},speed,callback);

          $("button").click(function(){
            $("div").animate({left: '250px'});
          }); 

          $("button").click(function(){
            $("div").animate({left: '250px'}, 1000, function(){
              alert('animation done!');
            });
          }); 
          ```
          [Try on w3schools](https://www.w3schools.com/jquery/tryit.asp?filename=tryjquery_animation1)


---


          #### jQuery effects - animate
  
          * jQuery animate() - Manipulate Multiple Properties

          ```JavaScript
          //  $(selector).animate({params},speed,callback);

          $("button").click(function(){
            $("div").animate({
              left: '250px',
              opacity: '0.5',
              height: '150px',
              width: '150px'
            });
          });
          ```

          [Try on w3schools](https://www.w3schools.com/jquery/tryit.asp?filename=tryjquery_animation1_multicss)


---


#### jQuery and DOM manipulation</h4>
          <ul>
            jQuery offers many DOM related methods that make it easy to:
              <ul>
                <li>Access and manipulate elements.</li>
                <li>Access and minpulate attributes.</li>
              </ul>
          </ul>

---


#### Three jQuery methods for DOM manipulation</h4>
          <ul>
            <li>text() - Sets or returns the text content of selected elements.</li>
            <li>html() - Sets or returns the content of selected elements (including HTML markup).</li>
            <li>val() - Sets or returns the value of form fields.</li>
          </ul>

---


####  jQuery - DOM manipulation

* Getting content and attributes

            ```HTML
            <div id="my-div">
              <p id="my-text">My Text</p>
              <input type="text" id="my-input" value="John Doe">
              <a id="my-link" href="https://www.google.com">google</a>
            </div>
            ```

            ```JavaScript
            $(document).ready(function(){
              console.log(('Text: ' + $('#my-text').text())); // Text: My Text
              console.log(('HTML: ' + $('#my-div').html())); // HTML: <p id="my-text">My Text</p> <input type="text" id="my-input" value="John Doe"> <a id="my-link" href="https://www.google.com">google</a>
              console.log(('Value: ' + $('#my-input').val())); // Value: John Doe
              console.log(('Attribute: ' + $('#my-link').attr('href'))); // Attribute: https://www.google.com
            });
            ```

            [Try on w3schools](https://www.w3schools.com/jquery/tryit.asp?filename=tryjquery_dom_html_get)


---


####  jQuery - DOM manipulation

* Setting content and attributes

            ```HTML
            <div id="my-div">
              <p id="my-text"></p>
              <input type="text" id="my-input" value="John Doe">
              <a id="my-link" href="https://www.google.com">google</a>
            </div>
            ```

            ```JavaScript
            $(document).ready(function(){
              $('#my-text').text('New Text');
              $('#my-input').val('New input value');
              $('#my-link').attr('href', 'https://www.bing.com'); // now google links goes to bing instead
            });
            
            $(document).ready(function(){
              $('#my-div').html('<h1>New h1</h1>');  // will overwrite and only add a h1
            });
            ```


---


####  jQuery - DOM manipulation - Adding new content

* ```append()``` = Inserts content at the end of the selected elements.
* ```prepend()``` = Inserts content at the beginning of the selected elements.
* ```after()``` = Inserts content after the selected elements.
* ```before()``` = Inserts content before the selected elements.



---


####  jQuery - DOM manipulation

            Initial HTML
            ```HTML
            <div id="my-div"></div>
            ```

            ```JavaScript
            $(document).ready(function(){
              $('#my-div').append('<p>Some appended text.</p>');
              $('#my-div').prepend('<p>Some prepended text.</p>'); 
              $('#my-div').after('<p>Some text after</p>');
              $('#my-div').before('<p>Some text before</p>');
            });
            ```

            Result
            ```HTML
            <p>Some text before</p>
            <div id="my-div">
              <p>Some prepended text.</p>
              <p>Some appended text.</p>
            </div>
            <p>Some text after</p>
            ```


---


####  jQuery - DOM manipulation

* Add Several New Elements With ```append()``` and ```prepend()```

            Initial HTML
            ```HTML
            <div id="my-div"></div>
            ```

            ```JavaScript
            $(document).ready(function(){
              let txt1 = '<p>Text.</p>'; 
              let txt2 = $('<p></p>').text('Text.');
              let txt3 = document.createElement('p');
              txt3.innerHTML = 'Text.';
              $('#my-div').after(txt1, txt2, txt3);  // Append the new elements
            });
            ```

            Result
            ```HTML
            <div id="my-div">
              <p>Text.</p>
              <p>Text.</p>
              <p>Text.</p>
            </div>
            ```


---
          

####  jQuery - DOM manipulation

* Add Several New Elements With ```before()``` and ```after()```

            Initial HTML
            ```HTML
            <div id="my-div"></div>
            ```

            ```JavaScript
            $(document).ready(function(){
              let txt1 = '<p>Text.</p>';
              let txt2 = $('<p></p>').text('Text.');
              let txt3 = document.createElement('p');
              txt3.innerHTML = 'Text.';
              $('#my-div').after(txt1, txt2, txt3); // Append the new elements
            });
            ```
            Result
            ```HTML
            <div id="my-div"></div>
            <p>Text.</p>
            <p>Text.</p>
            <p>Text.</p>
            ```


---


####  jQuery - DOM manipulation - Removing elements

* ```remove()``` - Removes the selected element (and its child elements)
* ```empty()``` - Removes the child elements from the selected element

            ```HTML
            <div id="my-div">
              <p>Hello World!</p>
            </div>
            ```

            ```JavaScript
            $(document).ready(function(){
              $('#my-div').remove();  // removes the <div> and <p> 
              
              $("#div1").empty(); // removes only the <p>
            });
            ```


---


####  jQuery & CSS'ing


* ```addClass()``` - Adds one or more classes to the selected elements
* ```removeClass()``` - Removes one or more classes from the selected elements
* ```toggleClass()``` - Toggles between adding/removing classes from the selected elements
* ```css()``` - Sets or returns the style attribute

            ```JavaScript
            $(document).ready(function(){
              $("#div1").addClass("important blue");  // adds classes blue and imortant
              $("h1, h2, p").removeClass("blue"); // removes class blue
              $("h1, h2, p").toggleClass("blue"); // toggles from having class blue and not having it
              console.log($("p").css("background-color")); // gets what bg color is has
              $("p").css("background-color", "yellow"); // sets background color to yellow
              $("p").css({"background-color": "yellow", "font-size": "200%"}); // sets multiple css properties
            });
            ```


---


#### AJAX & jQuery</h4>
##### jQuery Slim does not have AJAX functionality!</h5>
          <h6>Check your bootstrap import so that it is not the slim version!</h6>

---


####  AJAX & jQuery

* Loading external content.

            ```JavaScript
            $(selector).load(URL,DATA,CALLBACK);
            ```

* URL = file or external path
* DATA = 	key/value data is converterd to a string when sent
* CALLBACK 	= Function that runs when request is done


---



####  AJAX & jQuery

            ```JavaScript
            $(document).ready(function(){
              $('#div1').load('text.txt', function(responseTxt, statusTxt, xhr){
                if(statusTxt == 'success')
                  alert('External content loaded successfully!');
                if(statusTxt == 'error')
                  alert('Error: ' + xhr.status + ": " + xhr.statusText);
              });
            });
            ```

            ```HTML
            <div>
              Some text stored in the text.txt file..
            </div>
            ```


---


#### Callback parameters</h4>
          <ol>
            <li>responseTxt - contains the resulting content if the call succeeds.</li>
            <li>statusTxt - contains the status of the call.</li>
            <li>xhr - contains the XMLHttpRequest object.</li>
          </ol>

---


####  jQuery $.get() & $.post()

* The $.get() method requests data from the server with an HTTP GET request.
* The $.post() method requests data from the server using an HTTP POST request.

            ```JavaScript
            // The optional callback parameter is the name of a function to be executed if the request succeeds.
            $.get(URL,callback);

            // The optional data parameter specifies some data to send along with the request.
            // The optional callback parameter is the name of a function to be executed if the request succeeds.
            $.post(URL,data,callback);
            ```


---


####  jQuery $.get()

            ```JavaScript
            $(document).ready(function(){
              $.get('https://jsonplaceholder.typicode.com/users/1', function(data, status){
                console.log(data, status);  // Response object (already parsed) & 'success'
              });
            }); 
            ```


---


####  jQuery $.post()

            ```JavaScript
            $(document).ready(function(){
              $.post("https://jsonplaceholder.typicode.com/todos",
              {
                userId: 43,
                id: 33,
                title: 'Hello World!',
                completed: false
              },
              function(data, status){
                console.log(data,status);  // response object & 'success'
              });
            });
            ```


---


#### Pros and Cons jQuery vs JavaScript</h4>
            <ul>
              <li>Pros</li>
              <ul>
                <li>Eliminates a lot of cross browser javascript issues -> inconsistencies between browsers (browsers have become better over time).</li>
                <li>Can do more with less code.</li>
                <li>Easier to work with AJAX.</li>
                <li>Easy to get started with.</li>
              </ul>
              <li>Cons</li>
              <ul>
                <li>Overhead of adding extra javascript to page. (jQuery is quite small though).</li>
                <li>Multiple versions & Regular updates that change existing behaviour can be a risk.</li>
                <li>Might encourage people to not learn and understand the problems that jQuery solve.</li>
                <li>jQuery is  slower than CSS in many cases.</li>
              </ul>
            </ul>

---


#### To understand how jQuery works one needs to first know how JavaScript works.</h4>

---
        

### <a href="https://github.com/SofthouseVxo/Education" target="_blank">Github examples!</a></h3>

---
