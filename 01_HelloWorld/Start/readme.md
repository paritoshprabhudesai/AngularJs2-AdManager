
# Hello World Exampe Using Angularjs 2
#### 1.  Adding the root component
 * Add `app.component.ts`
``` typescript
            //import component from angular core
            import {Component} from 'angular2/core';
            
            //define the component 
            @Component({
                selector:'my-app',
                template:`<div ><h1>Hello World : {{pageTitle}}</h1>
                </div>`
            })
            
            //create class for the component
            export class AppComponent{
                pageTitle:string = "Angular 2";
            }
```
#### 2. Bootstraping the application
* Add `main.ts` file
```typescript
        // import bootstrap 
        import {bootstrap} from 'angular2/platform/browser';
        
        // import our component
        import {AppComponent} from './app.component';
        
        //bootstrap the component
        bootstrap(AppComponent);
```
#### 3. Call the directive in `index.html` file
* Call the directive in html page
```html
<body>
    <!--TODO: Add your component here-->
    <my-app>Loading...</my-app>
</body>
```
### 4. Open a command prompt in the project's root directory  (AngularJs2-AdManager\01_HelloWorld\Start)
* Type: `npm install` This installs the dependencies as defined in the package.json file.

* Type: `npm start` This launches the TypeScript compiler (tsc) to compile the application and wait for changes. It also starts the lite-server and launches the browser to run the application.