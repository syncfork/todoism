# Todoism

*We are todoist, we use todoism.*

> Example application for *[Python Web Development with Flask](https://helloflask.com/en/book/1)* (《[Flask Web 开发实战](https://helloflask.com/book/1)》).

Demo: http://todoism.helloflask.com

![Screenshot](https://helloflask.com/screenshots/todoism.png)

## Installation

clone:
```
$ git clone https://github.com/greyli/todoism.git
$ cd todoism
```
create & activate virtual env then install dependency:

with venv/virtualenv + pip:
```
$ python -m venv env  # use `virtualenv env` for Python2, use `python3 ...` for Python3 on Linux & macOS
$ source env/bin/activate  # use `env\Scripts\activate` on Windows
$ pip install -r requirements.txt
```
or with Pipenv:
```
$ pipenv install --dev
$ pipenv shell
```
init database then run:
```
$ flask initdb
$ flask translate compile
$ flask run
* Running on http://127.0.0.1:5000/
```

## License

This project is licensed under the MIT License (see the
[LICENSE](LICENSE) file for details).


# Windows
Download python 3.11 for windows
https://www.python.org/downloads/release/python-3119/ 

py -3.11 -m pip install -r requirements.txt

py -3.11 -m flask initdb
py -3.11 -m flask translate compile

Start 
py -3.11 -m flask run --port=5000

In case some error with the port:

netstat -ano | findstr :5000
then kill it:

taskkill /PID 1234 /F

Start 
py -3.11 -m flask run --port=5001
py -3.11 -m flask run