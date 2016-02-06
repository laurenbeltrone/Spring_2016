# Week 1 Instructor Notes

## Learning Targets
- I can explain when and why javascript is used.
- I can use the terminal to navigate, create files and folders.
- I can use javascript to store and compare data from a user.

## Do Now
- Open Slack (Browser or App!)
- In our class channel "js_driggers" slack your response to this question. What do you hope to accomplish in this class? Tag

## Introductions/Housekeeping

### Circle up! 2 whip arounds.
1. Name, Class, Major, Hometown, a movie you've seen 5+ times. 
2. Why JS? Why Now?

### Syllabus
- expectations
- long term goals
- on github
- contacting me
- contacting each other

### Diving In
####Ask what is JS?
- Javascript is not Java.
- Javascript is a programming language.
- Javascript is dynamic, change change at runtime.
- Javascript is untyped.

####Ask where is JS?
Javascript is nearly a universal language. It runs all sorts of devices and systems. Javascipt is in the browswer (client) and the server (node)

####Ask why JS?
- JS is the standard for all web interactions.
- JS is can be used as a full stack, meaning we can write js for both the client and the server. This is awesome!

## MiniLesson 1 - Using Terminal

## MiniLesson 2 - Javascript Data, Comparisons, Conditionals

### Variables and Datatypes
- Numbers, you know, 2, -5, 0.5, 54789
- Strings, Text! Always in quotes, single or double
- Boolean, True or False
- Arrays, Basically, a list. One direction exercises
- JS, null, undefined, NaN

#### Model, 15 minutes 
- go over taking in user input
- variables contain data (like my name is 'Pavan')
- variables can be initialized, then set
- if the variable is initialized, it's value is undefined, this is not good practice.
- you can do variable == undefined and it would be true
- undefined is a variable that's available in javascript on default (easy explaination)
- undefined is a variable that's available in global scope on default
- variables can be initialized and set in one go
- go over the different datatypes being used
- go over conditional logic 
- go over writing to the page

Example
```
	var userName = prompt("What's your name?");
			var confirm = confirm('Do you like cats?');

			var petName = 'Meeses';
			var petType = 'tuxedo cat';
			var petAge = 5;
			var petIsCat = true;

			if (confirm){
				alert(petName + petType + petAge)
			}else{
				alert("You don't get my cat's information")
			}

			if (petIsCat == true){
				alert('my pet is a cat')
			}else{
				alert('my pet is not a cat')
			}

			if (petAge !== 7){
				alert('My pet is not 7 years old')
			}

			if (petAge == 5){
				alert('My pet is 5 years old')
			}elseif(petAge < 5){
				alert('My pet is less than 5 years old')
			}elseif(petAge > 5){
				alert('My pet is older than 5 years old')
			}

			//this replaces the entire page with this - so it's not something you'll normally use - but it's what we'll use for now to be able to print stuff to the page
			document.write('Welcome to our page ' + userName);

			var catAge = prompt('how old is your cat?');

			alert(catAge + 2); //won't work as expected

			alert(parseInt(catAge) + 2); //works as expected
```

#### EX1 - 20 minutes
Write polling program. Ask for the user name, then ask for the voters age. If the user  is 18 or older, ask them who they will vote for from a list of options. Write to the screen their name, their age, and the candidate they chose.

If they younger than 18, alert them they can't vote.

**Bonus**
First ask the user if they are registered to vote. If yes continue with the first part. If no, redirect the user to the website to register in New York.

### EX2 - 5 minutes
Comparisons compare two things, give you an answer as a boolean value. Let's dig into some examples
	
```
		// discover exercise regarding strings, numbers and booleans, conditional logic

		
		/*
		if (true == true){
			alert('hi')
		}else{
			alert('bye')
		}*/

		/*
		if (false == false){
			alert('dude')
		}else{
			alert('nope')
		}*/

		/*if ("4" == 4){
			alert('barnard')
		}else{
			alert('marford - I made this up')
		}*/

		/*if ("4" === 4){
			alert('barnard')
		}else{
			alert('marford - I made this up')
		}*/

		/*if (true){
			alert('goo goo dolls')
		}else{
			alert('vanilla ice')
		}*/

		/*if (false){
			alert('the neighborhood')
		}else{
			alert('one direction')
		}*/

		/*if (("5" + "5") == "55"){
			alert('tofu')
		}else{
			alert('soybean')
		}*/

		/*if ((6 + "5") == "65"){
			alert('richard')
		}else{
			alert('branson')
		}*/
```

EX3
Ask the user if they are paying attention. If yes, respond wait 5 seconds, ask again! If they say no, tell them to wake up, wait 5 seconds, ask again!

this might break cause async! write and test

## Homework
Rock Paper Scissors, link to the github repo. Show how to use git classroom.





