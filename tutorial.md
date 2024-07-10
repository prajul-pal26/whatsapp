# basics
- django is the framework for building web application 
- with the help of django we can make API(application programming interface) ,which can connect with the client 

# features
- ORM object relational mapper
- the admin site
- caching 
- authentication 

# website

1 - front-end                                   2- Backend
-loaded on client machine                     - runs on a web server 
                                              - responsible for data processing 

# url - UNIFORM RESOURSE LOCATOR
  - LOCATE A  RESOURCE ON A INTERNET
  - RESOURCE - page
             - image 
             - video 
             - pdf
{        
[________url->_________browser->__________Browser_sends_a_request_to_web_server_which_hosted_a_website]
[server_take_this_request_process_it____________->return_response_back_to_the_client______]

## this data exchange is define by protocol called  -----HTTP(hyper text tranfer protocol)
# this define how server and client are communicate
}

# install
python -m venv myenv        [create_virtual_environment]
pip install django  [clone_django]
django-admin version                   [version_check]
django-admin startproject deep .        [start_project]
py manage.py startapp playground    [start_app]

django-admin    [to_check_all_the_commands_in_django]

django-admin runserver           [if_setting_is_set]
python manage.py  runserver              [same_as_above_without_setting]

#-------------------------------------------------------------------

INSTALLED_APPS = [
    'django.contrib.admin',    [#admin_interface_to_managing_or_data]
    'django.contrib.auth',            [#authenticate_the_user]
    'django.contrib.contenttypes',
    'django.contrib.sessions',      [#temperory_memory_on_the_server_for_managing_user_data]
                                [#not_used_so_we_can_dlt_this] 
    'django.contrib.messages',    [#used_for_one_time_notification_for_user]
    'django.contrib.staticfiles',   [#static_files_like_images_csv_and_so_on]
]


---------------------------------------------------------------------------
every time when you make app , please go to the setting in project and give name to the instal app  to it 

-----------------------------------------------------------------------------
# view section , 
-take a request and give a response
-request handler
-action


# url
map the url to the view funtion 

# templates
to return html content to the client(app)

# model 
to make a schema of the tables in the database,present in the app

# migration 
python manage.py migrations
python manage.py migrate

this is used to get updated in the database and django app

# connect to the database 
pip install psycopg2