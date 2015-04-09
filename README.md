# TransformationTool
Tool to transform input sources to RDF


## Requirements

* Make sure that Python 3.4 is installed, by executing the following command:
```shell
  python3
```
* Install the following packages:
```shell
  apt-get install python-virtualenv python3-dev
```
## Installation
* Create a new directory for the project:
```shell
  mkdir LindaTools
```
* Create a Python Virtual Environment with Python 3:
```shell
  virtualenv LindaTools --python=python3
  cd LindaTools
```
* Activate it (Needs to be done every time you work with it):
```shell
  source bin/activate
```
* Clone the repository:
```shell
  git clone https://github.com/LinDA-tools/TransformationTool.git
  cd TransformationTool
  git submodule init
  git submodule update
  git submodule foreach git checkout master
```
* Install the Requirements
```shell
  pip install -r requirements.txt
```
* Initialize the Database
```shell
  python manage.py migrate
  python manage.py syncdb
```
* Start the application
```shell
  python manage.py runserver
```
* Server is running now on: http://localhost:8000/
