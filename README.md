# provJewellery-cloud

Web service for managing handcrafted jewellery business process

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

* python 3.6
* [virtualenv](https://virtualenv.pypa.io/en/stable/)
* [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/install.html)
* pip3
* MySQL or any database
* [MySQL client](https://github.com/PyMySQL/mysqlclient-python) or any database client connector


### Installing

To install packages

```{shell}
pip install -r requirements.txt
```

Create a *.env* file on the root directory and pre-fill these variables. Secret key can be any hashed value.

```{shell}
SECRET_KEY=''

DATABASE_NAME=''
DATABASE_HOST=''
DATABASE_USER=''
DATABASE_PASSWORD=''
```

Then, inside your virtualenv make migrations and migrate

```{shell}
python manage.py makemigrations
python manage.py migrate
```

Once this is done, you can run the application

```{shell}
python manage.py runserver
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
