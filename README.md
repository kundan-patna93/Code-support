# Technical-suppoert
1)windows 7 service pack 1 and all applicable updates are required to install python 3.7.2

    Go this like download and install
    http://www.maxicsolutions.com/fixes/fix-windows-7-service-pack-error-python-3-5-higher

2)django-admin is not recognized as an internal or external command operable program or batch file

    step1:open the python idle
  
    step2:click the open and copy the addressbar to script 
  
    step3:this link is past the enviroment setting in the path
   
 3)MySQL shutdown unexpectedly.

    6:17:26 PM  [mysql] 	Error: MySQL shutdown unexpectedly.
    6:17:26 PM  [mysql] 	This may be due to a blocked port, missing dependencies, 
    6:17:26 PM  [mysql] 	improper privileges, a crash, or a shutdown by another method.
    6:17:26 PM  [mysql] 	Press the Logs button to view error logs and check
    6:17:26 PM  [mysql] 	the Windows Event Viewer for more clues
    6:17:26 PM  [mysql] 	If you need more help, copy and post this
    6:17:26 PM  [mysql] 	entire log window on the forums

    Step1: Open XAMPP and click the services
    Step2: Open the services tab and find our MySQL80 and open it
    Step3: open new tab press the stop butoom and restart XAMPP 

4)How to Install Django in Virtual Environment.

    following step:
    step1:Open cmd
        win+r-->cmd
        
    setp2:Install Virtual Enviroment Wrapper
        pip install virtualenvwrapper-win
        
    step3:Create Virtual Environment(VE)
        mkvirtualenv <foldername>
        
    step4:Install django
        pip install django==<version name>

5)TypeError: unsupported operand type(s) for /: 'str' and 'str'

    DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        #'NAME': BASE_DIR / 'db.sqlite3',               comment this line of code or remove
        'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),   add this line of code
    }
   }




6)TemplateSyntaxError at /
  'staticfiles' is not a registered tag library. Must be one of:
  
  
    if you write this one :
    {% load staticfiles %} #remove this

    Then remove upper code and write below code 
    {% load staticf %} #use this one
    
7)How to Indent and Dedent Your Python Code


    Indent- ctrl+]
    Deindent- ctrl+[
