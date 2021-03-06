## Instructions

### Logins
#### Main

1. danilenko
2. egorenko
3. liygin
4. maliygin
5. mashrapov
6. nosulia
7. pinkin
8. poliakov
9. pronina

####Additional

1. monkey1
2. monkey2
3. monkey3
4. monkey4
5. monkey5

### Putty

#### Installation

[Download Putty](https://the.earth.li/~sgtatham/putty/latest/x86/putty.exe)

#### Set a session

1. Session - Host: 194.87.236.197
2. Connection - Data - Auto-login username: [your_login]
3. Session - Saved Sessions: [your_login]_eduserv
4. Session - Saved Sessions - Save
5. Session - Open

### Virtualenvwrapper with python 3
#### Installation

`pip3 install virtualenvwrapper`

#### Settings

1. `nano ~/.bashrc`
2. Insert into the end of the file: 

  `VIRTUALENVWRAPPER_PYTHON='/usr/bin/python3' 
  `source /usr/local/bin/virtualenvwrapper.sh`
  
3. CTRL+X, ENTER
4. `exit`  # You should relogin

#### Virtual environment

1. Create a folder projects in your home directory
2. Create a folder [project_name] in the projects folder
3. `mkvirtualenv -a /home/[your_login]/projects/[project_name] [project_name]`
4. `deactivate`

#### Exercise

1. `workon [project_name]`
2. `pip3 install requests`
3. `pip3 install numpy`
4. `pip3 freeze > requirements.txt`
5. Look at content of the requirement.txt file
6. `deactivate`
7. `pip3 freeze > requirements_global.txt`
8. Look at content of the requirement_global.txt file
9. Create new folder [second_project]
10. Copy the requirements.txt file to the [second_project] directory 
11. Create a new virtual environment [second_project] linked to the [second_project] directory 
12. Activate new virtual environment [second_project]
13. `pip3 install -r requirements.txt`
14. `pip3 freeze > requirements_second_project.txt`
15. Look at content of the requirements_second_project.txt file


### WinSCP
#### Installation

[Download WinSCP Portable](https://winscp.net/download/WinSCP-5.9.2-Portable.zip)

#### Set a session

1. Host name: 194.87.236.197
2. User name: [your_login]
3. Password: [your_password]
4. Save
5. Login

#### Exercise

1. Copy a folder with files requirements.txt and requirements_global.txt to your local machine.
