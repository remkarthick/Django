# Setting up Environment

1. Install Python inside C:\KK\Programs\python\python39 folder

2. Install pipenv inside the python

    pip install pipenv

3. Create a new folder named LearnDjango. 

4. Create a new batch file in a LearnDjango folder with the below content

    path =%path%;C:\KK\Programs\python\python39;C:\KK\Programs\python\python39\Scripts;
    start cmd .


5. Open the batch file and Check if we are in a virtual environment

    pipenv --venv

> Example : C:\KK\learn\python\LearnDjango>pipenv --venv No virtualenv
> has been created for this project(C:\KK\learn\python\LearnDjango) yet!
> Aborted!

6. Create / Get into the virtual environment

    pipenv shell

> Example :
> 
> C:\KK\learn\python\LearnDjango>pipenv shell 
> Creating a virtualenv for
> this project... Pipfile: C:\KK\learn\python\LearnDjango\Pipfile Using
> C:/KK/Programs/python/python39/python.exe (3.9.5) to create
> virtualenv... [=== ] Creating virtual environment...created virtual
> environment CPython3.9.5.final.0-64 in 4011ms   creator
> CPython3Windows(dest=C:\Users\<username>\.virtualenvs\LearnDjango-u7fHf1rZ,
> clear=False, no_vcs_ignore=False, global=False)   seeder
> FromAppData(download=False, pip=bundle, setuptools=bundle,
> wheel=bundle, via=copy,
> app_data_dir=C:\Users\<username>\AppData\Local\pypa\virtualenv)
>     added seed packages: pip==22.2.2, setuptools==65.3.0, wheel==0.37.1   activators
> BashActivator,BatchActivator,FishActivator,NushellActivator,PowerShellActivator,PythonActivator
> 
> Successfully created virtual environment! Virtualenv location:
> C:\Users\<username>\.virtualenvs\LearnDjango-u7fHf1rZ Creating a
> Pipfile for this project... Launching subshell in virtual
> environment... Microsoft Windows [Version 10.0.19044.2006] (c)
> Microsoft Corporation. All rights reserved.
> 
> (LearnDjango-u7fHf1rZ) C:\KK\learn\python\LearnDjango>

7. Check if we are in the virtual env

    pipenv --venv

> Example : (LearnDjango-u7fHf1rZ) C:\KK\learn\python\LearnDjango>pipenv --venv 
> C:\Users\<username>\.virtualenvs\LearnDjango-u7fHf1rZ

8. Check if there is any packages installed in the Virtual Environment

    pip freeze
   
9. Install django inside the Virtual Environment

    pipenv install Django==3.0.
    
> Example :
> 
>  (LearnDjango-u7fHf1rZ) C:\KK\learn\python\LearnDjango>pipenv install Django==3.0.8 
> Installing Django==3.0.8... Adding Django to Pipfile's
> [packages]... Installation Succeeded Pipfile.lock not found,
> creating... Locking [packages] dependencies...
>            Building requirements... Resolving dependencies... Success! Locking [dev-packages] dependencies... Updated Pipfile.lock (13ff3d)!
> Installing dependencies from Pipfile.lock (13ff3d)...

10. Check if Django is installed in the Virtual Environment

    pip freeze

> Example :
> 
> (LearnDjango-u7fHf1rZ) C:\KK\learn\python\LearnDjango>pip freeze
> asgiref==3.5.2
> Django==3.0.8
> pytz==2022.4
> sqlparse==0.4.3
