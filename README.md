# Code-support
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
    
    
8)Auto complete html basic structure

    1. Sublime text - html + tab 
    2. vs code      - ! + tab(if not work then followed below step
        step-1: open vs code
        step-2: enter ctrl+ship+p ->type User setting
        step-3: type emmet ->scroll down
        step-4: enable ->show Suggestions As Snippets
                enable ->Trigger Expansion On Tab
                
       step-5: Restart vs code
       https://www.youtube.com/watch?v=k8IyBpaDEr8
    
    
   9)I'm not able to install ChatterBot library by using command "pip install chatterbot". Can anyone help me with this issue?
   
        =>
        1. pip install chatterbot==1.0.0
        2. pip install chatterBot-corpus
        In case if the Above don't work... Use pip3 instead of pip.
        
        =>AttributeError: module 'time' has no attribute 'clock'
          import time
          time.clock = time.time
          
       =>No value for search_text was available on the provided input
         import logging
         logger = logging.getLogger()
         logger.setLevel(logging.CRITICAL)
         
   10)Json validation online site.
   
        https://codebeautify.org/jsonvalidator
        
   11)Odoo_15 Problem( Error: EPERM: operation not permitted, mkdir 'c:\Program Files\Odoo-15\server\odoo\addons\kundan' )
   
        The folder > Properties > Security Tab
        Edit > select the user and give full control
        
  12)Django html and css link code:
        
        Note:
        templates
        static
        
        HTML:
        setting.py
        import os
        TEMPLATE_DIR =os.path.join(BASE_DIR,'templates') 
        
        templates:
        DIR=[]
        os.path.join(BASE_DIR,'templates'
        
        
        
        CSS:
        1:html page:
        <!DOCTYPE html>
        {% load static %}
        
        2:link css:
        <link rel="stylesheet" href="{% static "css/login.css" %} " />
        <title>login Page</title>
        
        3:setting code:
        STATIC_DIR = [os.path.join(BASE_DIR,'static')]
        
   14)dict key rename:
   
       dic[new_key]=dic.pop(old_key)
       
   15)fuction called another name:
   
       def show_record(name):
            print(name)
       
       show_record(name="sunil")
       display_record=show_record
       display_record(name="krishana")
       
   16)Mysql connection test:
   
       if conn.is_connected():
            print("successfull connected...!")
            
            
   17)HTML Skeleton in sublime text Editor:
   
   
       html + TAB press
        
 
          
         
         

        
        
   
   
        
    
    
    
    
    
    
    
