https://github.com/angular/angular-cli

ng generate component my-new-component
ng g component my-new-component # using the alias

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
		
		
		
