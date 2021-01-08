# django-password
Password Generator 
This project will help user to choose randomized password with capitalized and numerical options.

Create Project:
"	Go to terminal/Bash Operator, type cd Desktop (or you can choose any direction to save your project). 
"	On your terminal/Bash Operator, Django-admin startproject name of your project.
"	Once you created new project you can test it to see if it's working fine, go to terminal/Bash Operator python manage.py runserverí copy link below usually its localhost:8080 past it to your url browser. You should see your very first Django page which is running by default. 
"	Now you can choose which code-editor you can use for project, i use Atom, but there are plenty other ones which can be useful as well. Open your code-editor and add your project. 
"	On your left hands-side you will find setting.py í go to setting.py í go to App Installed í add your app name. 
"	Step to remember, when user types www.example.com this request first goes to Url.py and look for matching name or path, once it finds matching path, url transfers this to views.py (place where all complex python codes are written). 
"	Import  from your app import views. Crete first path("example", views.example)
"	Go to Views.py í import from django.http import HttpResponse.
"	Go to Views.pyí create function such as: def example(request):
                                                                                                           return HttpResponse(<h1> Hello World </h1> )
"	Go to your Terminal í python manage.py runserverí try localhost:8080/example. You should see message (Hello World).
"	Now the page is working fine, but if we want to add more functionalities to your page, using HttpResponse inside View.py can mix-up your codes and you might eventually get bugs. 

Create Templates:

Templates are convenient and clean way to store your HTML codes. Templates is final step before user gets response as Web-Page.

"	Rigth click to your app-name to create Templates file,  app-name/templates/app-name/example.html. 
"	Go to your template and write <h1> Hello World </h1> {{ example }}
"	Go to Views.py and edit your function: def example(request):
                                                                                                     return render(request, 'app_name/example.html', {'example'/'example.html'}) 
"	Try to re-run your page one more time, you should be able to see the same result as before. Now you can see that we moved HTML code into templates and get the same message. 

