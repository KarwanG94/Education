<!doctype html>
<html>
	<head>
    <title>Angular HTTP</title>
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

#### 12. Angular</h4>
##### HttpClient & RxJS basics</h5>

---


          <h2 style="color: #D81B60;">RxJS</h2>
#### Reactive Extensions</h4>

---
        

#### Purpose of this lecture</h4>
          <ul>
            <li>To grasp some overall RxJS concepts and to be able to use Angulars HttpClient in a basic way.</li>
            <li>Not to be a RxJS pro, we could have spent weeks expoloring RxJS itself.</li>
          </ul>

---


#### RxJS</h4>
					<ul>
						<li>Reactive Extensions library for JavaScript</li>
						<li>Is standalone library which Angular uses.</li>
            <li>RxJS is a dependency, check package.json.</li>
            <li><a href="https://rxjs-dev.firebaseapp.com/guide/overview" target="_blank">RxJS Documentation</a></li>
					</ul>

---
        

          <p>"RxJS is a library for composing asynchronous and event-based programs by using observable sequences." - <a href="https://rxjs-dev.firebaseapp.com/guide/overview" target="_blank">RxJS Documentation</a></p>

---


					<img src="/new/media/pushpull2.png" alt="push and pull">

---


#### What is Pull?</h4>
          <ul>
            <li>"In Pull systems, the Consumer determines when it receives data from the data Producer. The Producer itself is unaware of when the data will be delivered to the Consumer."  - <a href="https://rxjs-dev.firebaseapp.com/guide/observable">RxJSDocumentation</a></li>
            <li>"Every JavaScript Function is a Pull system. The function is a Producer of data, and the code that calls the function is consuming it by "pulling" out a single return value from its call." - <a href="https://rxjs-dev.firebaseapp.com/guide/observable">RxJSDocumentation</a></li>
          </ul>

---


#### What is Push?</h4>
          <ul>
            <li>"What is Push? In Push systems, the Producer determines when to send data to the Consumer. The Consumer is unaware of when it will receive that data." - <a href="https://rxjs-dev.firebaseapp.com/guide/observable">RxJSDocumentation</a></li>
            <li>"Promises are the most common type of Push system in JavaScript today. A Promise (the Producer) delivers a resolved value to registered callbacks (the Consumers), but unlike functions, it is the Promise which is in charge of determining precisely when that value is "pushed" to the callbacks." - <a href="https://rxjs-dev.firebaseapp.com/guide/observable">RxJSDocumentation</a></li>
          </ul>

---


#### Essential concepts</h4>
          <ul>
            <li>Observable: represents the idea of an invokable collection of future values or events.</li>
            <li>Observer: is a collection of callbacks that knows how to listen to values delivered by the Observable.</li>
            <li>Subscription: represents the execution of an Observable, is primarily useful for cancelling the execution.</li>
            <li>Operators: are pure functions that enable a functional programming style of dealing with collections with operations like map, filter, concat, flatMap, etc.</li>
            <li>Subject: is the equivalent to an EventEmitter, and the only way of multicasting a value or event to multiple Observers.</li>
            <li><a href="http://reactivex.io/rxjs/manual/overview.html#introduction">RxJSDocumentation</a></li>
          </ul>

---


#### Observables</h4>
          <p>RxJS introduces Observables, a new Push system for JavaScript. An Observable is a Producer of multiple values, "pushing" them to Observers (Consumers).</p>
          <ul>
            <li>A Function is a lazily evaluated computation that synchronously returns a single value on invocation.</li>
            <li>A generator is a lazily evaluated computation that synchronously returns zero to (potentially) infinite values on iteration.</li>
            <li>A Promise is a computation that may (or may not) eventually return a single value.</li>
            <li>An Observable is a lazily evaluated computation that can synchronously or asynchronously return zero to (potentially) infinite values from the time it's invoked onwards.</li>
          </ul>

---


            ### Declaring an Observable
            ```JavaScript
            var observable = Rx.Observable.create(function (observer) {
              observer.next(1);
              observer.next(2);
              observer.next(3);
              setTimeout(() => {
                observer.next(4);
                observer.complete();
              }, 1000);
            });
            ```


---


            ### Eventlisteners & Observables
            ```JavaScript
            var button = document.querySelector('button');
            button.addEventListener('click', () =>    console.log(’Clicked!’)
            );
            ```

            Using RxJS you create an observable instead.
            ```JavaScript
            var button = document.querySelector('button');

            Rx.Observable.fromEvent(button, 'click')
              .subscribe(() => console.log('Clicked!'));
            ```


---


  <img src="/new/media/promisevsobs.png" alt="observable vs promise">

---


            ### Observer

            An Observer is a consumer of values delivered by an Observable. Observers are simply a set of callbacks, one for each type of notification delivered by the Observable: next, error, and complete.

            ```JavaScript
            var observer = {
              next: x => console.log('Observer got a next value: ' + x),
              error: err => console.error('Observer got an error: ' + err),
              complete: () => console.log('Observer got a complete notification'),
            };
            ```
            Observers are just objects with three callbacks, one for each type of notification that an Observable may deliver.
            <a href="http://reactivex.io/rxjs/manual/overview.html#observer">RxJSDocumentation</a>


---


            ### Subscribing

            Subscribing to an Observable is like calling a function, providing callbacks where the data will be delivered to.

            A Subscription essentially just has an unsubscribe() function to release resources or cancel Observable executions.
            ```JavaScript
            var observable = Rx.Observable.interval(1000);
            var subscription = observable.subscribe(x => console.log(x));
            // Later:
            // This cancels the ongoing Observable execution which
            // was started by calling subscribe with an Observer.
            subscription.unsubscribe();
            ```
            <a href="http://reactivex.io/rxjs/manual/overview.html#subscription">RxJSDocumentation</a>


---


            ### Subjects
            An RxJS Subject is a special type of Observable that allows values to be multicasted to many Observers.

            While plain Observables are unicast (each subscribed Observer owns an independent execution of the Observable), Subjects are multicast.

            Subjects are like EventEmitters: they maintain a registry of many listeners.



---
        <section data-markdown>
            <script type="text/template">
          ```JavaScript
          var subject = new Rx.Subject();

          subject.subscribe({
            next: (v) => console.log('observerA: ' + v)
          });
          subject.subscribe({
            next: (v) => console.log('observerB: ' + v)
          });

          subject.next(1);
          subject.next(2);
          ```


---


#### Operators</h4>
          <ul>
            <li>Most operators operate on an Observable and return an Observable. This allows you to apply these operators one after the other, in a chain.</li>
            <li><a href="http://reactivex.io/documentation/operators.html">Complete list</a></li>
          </ul>

---
				

#### Observables in Angular</h4>
          <ul>
            <li>The EventEmitter class extends Observable.</li>
            <li>The HTTP module uses observables to handle AJAX requests and responses.</li>
            <li>The Router and Forms modules use observables to listen for and respond to user-input events.</li>
          </ul>

---


#### HttpClient</h4>
          <p>Angular’s HttpClient returns observables from HTTP method calls.</p>
          <ul>
            <li>HTTP requests are cancellable through the unsubscribe() method.</li>
            <li>Requests can be configured to get progress event updates.</li>
            <li>Failed requests can be retried easily.</li>
          </ul>

---


####  HttpClientModule
            ```JavaScript
            import { HttpClientModule } from '@angular/common/http';

            imports: [
              BrowserModule,
              AppRoutingModule,
              FormsModule,
              HttpClientModule
            ]
            ```


---


#### Angular HttpClient</h4>

          <ul>
            <li>Simplified client HTTP API for Angular applications that rests on the XMLHttpRequest interface exposed by browsers.</li>

            <li>Observable API's, and streamlined error handling.</li>
          </ul>

---


#### HttpClient</h4>
          <ul>
            <li>.get ()</li>
            <li>.post ()</li>
            <li>.put ()</li>
            <li>.delete ()</li>
          </ul>

---


  <img src="/new/media/get.png" alt="get n stuff">
          <p></p>

---

  <img src="/new/media/put.png" alt="put n stuff">

---


### Check Examples on Github!</h3>

---

