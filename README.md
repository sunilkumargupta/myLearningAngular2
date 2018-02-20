Step 1: install nodejs
		https://nodejs.org/en/

Step 2: npm install -g @angular/cli
		https://github.com/angular/angular-cli		
		
Wow ------------- All set--------

for my reference .. I am going to create new App with routing module + Lazy loaded modules + Service + AuthGaurd

1.
ng new myLearning --routing

2.
ng g guard auth-gaurd --module=app.module

3.
ng g module s-component --routing --module=app.module			--to create a new module
ng g module html-video --routing --module=app.module


4.
ng g c help -d
ng g c help --flat -d
ng g component s-component/sdialog -d
ng g component s-component/sdialog --flat -d
ng g component s-component/sdialog --flat --spec=false -d

ng g c help --flat
ng g component s-component/sdialog --flat


<for inline template & inline css>
ng g c help --flat -it -is --spec=false -d

<for scss instead of css>
ng g c help --style=scss



5.
ng g s services/user --module=app.module
ng g s services/user -m=app.module
ng g s services/user -m=app.module --flat=false
ng g s services/backend -m=s-component/s-component.module

6. create class/
	a. class
		ng g cl model/UserDto 
		[ we can do dry run without actually creating the same: ng g cl model/UserDto -d]
	
	b. Interface
		ng g i model/IUserDto
		
	c. enum
		ng g e model/UserType








===========================================================

--spec: boolean, default false, generate spec file with unit test

-----------------------------------------------
ng new myLearning --routing -si [Skip install]




========================================================================
https://github.com/angular/angular-cli
https://www.sitepoint.com/ultimate-angular-cli-reference/
https://www.youtube.com/watch?v=54lvXWA3U-g



ng generate component my-new-component
ng g component my-new-component # using the alias
<pre>
# components support relative path generation
# if in the directory src/app/feature/ and you run
ng g component new-cmp
# your component will be generated in src/app/feature/new-cmp
# but if you were to run
ng g component ./newer-cmp
# your component will be generated in src/app/newer-cmp
# if in the directory src/app you can also run
ng g component feature/new-cmp
# and your component will be generated in src/app/feature/new-cmp
</pre>

You can find all possible blueprints in the table below:

Scaffold	Usage
Component	ng g component my-new-component
Directive	ng g directive my-new-directive
Pipe		ng g pipe my-new-pipe
Service		ng g service my-new-service
Class		ng g class my-new-class
Guard		ng g guard my-new-guard
Interface	ng g interface my-new-interface
Enum		ng g enum my-new-enum
Module		ng g module my-module


===============================================================

1. ng new myApp   or 	ng new myApp --routing
2. cd myApp
3. Component:
	ng g c protal
4. Service:
	a. ng g s protal
	b. it is possible to provide the service (or guard, since that also needs to be provided) when creating the service.
		The command is the following...
		ng g s services/backendApi --module=app.module
	c. It is possible to provide to a feature module, as well, you must give it the path to the module you would like.
		ng g s services/backendApi --module=services/services.module
		
		
		
