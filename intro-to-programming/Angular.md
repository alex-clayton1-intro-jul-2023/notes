
- Angular is the default to make it easy to transfer new developers to different projects. Good for making things run in a web browser.
	- Angular is very opinionated
	- The project structure, naming conventions, etc. are fairly consistent from one application to another.
	- React is good because everything is tweakable. A lot more customization.
	- Angular provides a fairly similar experience for every application.
		- Angular has UI library called CoreUI. Has a date-picker that has the same thing for across all the projects.

*To Create an Angular Application* #angular
- Angular Command Line Interface (Angular CLI) [Angular - CLI Overview and Command Reference](https://angular.io/cli)
	- Install it with:
		- `npm install --global @angular/cli@latest
		- `npm i -g @angular/cli@latest`
			- If you leave latest off, it assumes latest version. Otherwise can specify version after @
		- `ng new app --standalone --skip-git --skiptests`
			- Yes to routing
			- default css
		- Can always have a browser open that shows the current app
			- `ng serve -o`
				- the -o makes it open automatically for you
				- Must run in the folder with angular app

*Angular File Structure* #angular 
	- app.component.html has some stuff defined in there
		- Make sure to import components in here
	- Header.component.ts
		- Component file is structured  with
		- `export class HeaderComponent`
		- Before that component must be defined
			- Component must be imported from Angular
				- `import { Component } from "@angular/core";`
				- Define component as `standalone: true`

- Angular #angular 
	- NOT for creating websites or webpages
	- This is used for creating applications that download and build within a web browser
	- Written in Typescript #ts
		- Typescript compiles to JavaScript
		- TypeScript wants to address how JavaScript can change types for a variable.
		- Gets rid of lots of requirement for testing
	- Tool for creating User Interfaces
	- All file names MUST be undercase #qa

	- *Component*
		- A typescript class
		- A template
		- Both of these are compiled and sent to the browser
	-  *A component has two jobs:*
		- Accurately project the application *state*
			- State: The value of all meaningful data NOW.
		- Provide affordances through which the user can interact with the application
			- A component 
		- Generate components by creating typescript class #ts
	- *Page*
		- Pages are things you route to
		- Components are other things