# Angular-Introduction
</br>
1)a)Create two new Components (manually or with CLI): WarningAlert and SuccessAlert </br>
b)Output them beneath each other in the AppComponent </br>
c)Output a warning or success message in the Components </br>
d)Style the Components appropriately (maybe some red/ green text?) </br>

Briefly I need this: </br>

![image](https://user-images.githubusercontent.com/110709552/202995399-549f3317-bd08-4205-893b-1b1979688a84.png)

2)I need When button clicked change below text to "Server was created". Use string Interpolation and event binding.
![image](https://user-images.githubusercontent.com/110709552/202997090-952e1fdf-92f1-483e-a104-6ed7326fd954.png) </br>

3) Create a Component which you are going to use it in root component. Inside a custom component I need you to create a button. When page is executed, button supposed to be disabled and after 2 seconds it is going to be enabled automatically. (Use again data binding especially property one.)

-----

<h1>Some Informations to know:</h1> </br>

The CLI generates a different welcome screen than you're going to see in my video though. No worries, you'll still be able to follow along without issues! Just make sure to code along so that your code equals mine - Angular itself didn't change a bit :)

-----

If you want to dive deeper into the CLI and learn more about its usage, have a look at its official documentation: https://github.com/angular/angular-cli/wiki

You encountered issues during the installation of the CLI or setup of a new Angular project?

A lot of problems are solved by making sure you're using the latest version of NodeJS, npm and the CLI itself.

Updating NodeJS:

Go to nodejs.org and download the latest version - uninstall (all) installed versions on your machine first.

Updating npm:

Run [sudo] npm install -g npm  (sudo  is only required on Mac/ Linux)

Updating the CLI

[sudo] npm uninstall -g angular-cli @angular/cli 

npm cache verify 

[sudo] npm install -g @angular/cli 

Here are some common issues & solutions:

Creation of a new project takes forever (longer than 3 minutes)
That happens on Windows from time to time => Try running the command line as administrator

You get an EADDR error (Address already in use)
You might already have another ng serve process running - make sure to quit that or use ng serve --port ANOTHERPORT  to serve your project on a new port

My changes are not reflected in the browser (App is not compiling)
Check if the window running ng serve  displays an error. If that's not the case, make sure you're using the latest CLI version and try restarting your CLI

-----

One important note: All the course code will only work if you are NOT using "strict mode" see the "First App" lecture in this module. Strict mode forces you to write more verbose code in some places (especially when it comes to class properties). If you enabled it by accident, you can also disable it by setting strict: false in your tsconfig.json file.

---

Due to dependency version mismatches, running the attachments might fail though - in that case, you can try the following:

1) Create a new project via ng new my-project --strict false (the --strict false part is important!)

2) Copy the content of the ZIP attachment src/app folder into the newly created project src/app folder.

3) Run your project (my-project) via ng serve

If you try to directly run my ZIP attachments, you must run npm install first.

If you're getting errors when running npm install, you can often solve them by running npm install --legacy-peer-deps instead of npm install.

