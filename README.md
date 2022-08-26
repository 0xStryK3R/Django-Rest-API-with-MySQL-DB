## Django Rest API Example with MySQL DB

***
[Course Link](https://www.udemy.com/course/api-engineer-node-python-django-postman-postgresql/learn/lecture/27436790#overview)

***
> In case of ***'2026, SSL connection error: unknown error number'*** errors while doing db migrate follow stpes [here](https://stackoverflow.com/questions/68914963/2026-ssl-connection-error-unknown-error-number-encountered-by-my-django-app) or as mentioned below:

1. Install pymysql:
    ```console
        python -m pip install pymysql
    ```

2. Add below line to projects `init.py` file (in same directory as `settings.py`)
    ```python
    import pymysql
    pymysql.install_as_MySQLdb()
    ```