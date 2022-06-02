# OnlineFoodOrdering
**Spec:**
  - Web Framework: Django 2.2
  - Database Server: PostgreSQL 12.3
  
**How to run:**
 - Clone the [github repo]([https://github.com/AnshDesai/Online-Food-Ordering])
**Python Environment/Database setup**
        - install postgres database
        - create a new database in your postgres server named `foodsquare` with owner as `postgres`, password as  `postgres`   
        - start the postgres server on port 5432 
        - move to the project directory 
        - create a virtual environment & activate it
        ```shell
        python3 -m pip install --upgrade pip
        python3 -m venv venv
        source venv/bin/activate
        ```
        - install dependencies & make migrations
        ```shell
        python3 -m pip install -r requirements.txt
        python3 manage.py makemigrations
        python3 manage.py migrate
        ```
        - now run the server finally
        ```shell
        python3 manage.py runserver
        ```
        - now browse the site at http://localhost:8000/ 
        - **N.B.** a facebook login app needs to be set up & its credentials are to be addded into database properly to access login pages.  
          For ease, an app is created & its credentials are provided into a dumped json file which can be loaded into the database using:
        ```shell
        python3 manage.py loaddata data.json
        ```
 - **N.B.** Facebook/Google login may not work properly as those login apps credentials might be outdated now.          
          
          
**Some Basic Functionalities Implemented:**
- User Session Handling
- Third Party Authentication
- Sub-domain Handling
- Shopping Cart Management
- Local Storage Handling
- Online Payment Handling
- Review-Rating Management

***
## Sample Usage:

***Browse Cuisines***
![Browse Cuisines](https://github.com/AnshDesai/Online-Food-Ordering/blob/master/Foodsquare_Screenshots/filter.png)

***Payment***

<img src="https://github.com/AnshDesai/Online-Food-Ordering/blob/master/Foodsquare_Screenshots/bkash.png" alt="Payment" width="500" height="400"/>

***Branch Open***
![Branch Open](https://github.com/AnshDesai/Online-Food-Ordering/blob/master/Foodsquare_Screenshots/rest_branch_reg.png)
***Add Items***
![Add Items](https://github.com/AnshDesai/Online-Food-Ordering/blob/master/Foodsquare_Screenshots/additem.png)

***Manage and Accept Orders***
![Manage and Accept Orders](https://github.com/AnshDesai/Online-Food-Ordering/blob/master/Foodsquare_Screenshots/accept_branch.png)
