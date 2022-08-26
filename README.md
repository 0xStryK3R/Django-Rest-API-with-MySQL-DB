## Sample Django Rest API Project with MySQL DB | ![Visitor Count](https://visitor-badge.glitch.me/badge?page_id=0xStryK3R.Django-Rest-API-with-MySQL-DB)

***
### Setup Commands:

1. Setup the Database and DB User via MySQL Workbench.

2. Clone Git-Repo into Local Directory.

3. Update DB credentials in _`settings.py`_ file in _`.\worldCountries\`_ folder to as per your own configuration.

4. Open Command Line in main directory of project.

5. Run below command inside project directory to setup environment
      ```console
      python -m venv .venv
      ```
6. Activate enviroment with below command (for Windows):
      ```console
      .venv\Scripts\activate
      ```
7. Run below command next to install required modules plus dependencies defined in `requirements.txt`
      ```console
      pip install -r requirements.txt
      ```
8. Migrate default/admin tables:
      ```console
      python manage.py makemigrations
      python manage.py migrate
      ```
9. Create a super user(admin) for your project:
      ```console
      python manage.py createsuperuser
      ```
      > _**Note:** This user is used to manage administration for your project via the admins console: [`/admin`](http://localhost:5000/admin/)._

10. Insert some data into the newly created _`countries`_ table.
    
11. Run the project:
    ```console
    python manage.py runserver 0.0.0.0:5000
    ```    
12. All Done!! [`Click Here`](http://localhost:8000/api/countries) or use Postman to interact with your app.

> _**Assumptions**: Python and MySQL has been setup and running prior to starting with this project._

> _**References**: For Complete details, please refer [`API Engineer: Node | Python | Django | Postman | PostgreSQL`](https://www.udemy.com/course/api-engineer-node-python-django-postman-postgresql/learn/lecture/27436790#overview) - the source material for this Repo._
