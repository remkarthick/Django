# install pipenv

1. Open the Python installed folder
   - C:\KK\Programs\python\python39
2. Open the Scripts folder inside the python installed folder
   - C:\KK\Programs\python\python39\Scripts
3. Open the cmd prompt inside the above folder and type the below command 
   - pip install pipenv
4. Inside the pycharm installed folder, create a new batchfile named kkpycharm.bat and below should be its content

	`path=%path%;C:\KK\Programs\python\python39;C:\KK\Programs\python\python39\Scripts;
	start pycharm64.exe`
5. Open the pycharm using our new batch file, Create a new project selecting the "C:\KK\Programs\python\python39\python.exe" as interpreter
6. Run the below command within the pycharm terminal
  - `pipenv shell`
  
# If you get the below error
 
`Usage: pipenv shell [OPTIONS] [SHELL_ARGS]...

ERROR:: --system is intended to be used for pre-existing Pipfile installation, not installation of specific packages. Aborting.
`

then get the existing virtual env info using the below command

`pipenv --venv`

`
C:\Users\<username>\.virtualenvs\Django-0849uI4V
`

remove the folder

rm -rf C:\Users\<username>\.virtualenvs\Django-0849uI4V

re create the virtual env

# Remake virtualenv
cd C:\KK\learn\python\Django
`pipenv --python 3`
(or)
`pipenv shell`

# View the current location of virtual environment

`pipenv --venv`

# View the contents of the virtual environment

`pip freeze`

# Get inside the virtual environment

`pipenv shell`

# Install package inside virtual environment

`pipenv install pytest`
