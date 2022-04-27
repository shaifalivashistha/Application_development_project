<u><h2 align="center">REPORT</h1></u>

***Author :***
- *<u>Name</u>*- Shaifali Vashistha
- *<u>Roll number</u>*- 21f1003257
- *<u>Student email</u>*- 21f1001231@student.onlinedegree.iitm.ac.in. 
- *<u>Details</u>*- Along with this course I am pursuing BSc in Zoology and Botany from Model Public College, Chandausi. I have a keen interest in exploring the different realms of Technology and thus I wish to accomplish this degree with utmost dedication and hard work.

**Description :**

In this project I have designed Self Tracker Application with 2 kinds of tracker- Numeric, Boolean which will track progress over time and shows graphs (wherever applicable). Each tracker has its own ID, description and displays the log in time, value (based on the corresponding tracker type) and accordingly a note entered by the user. User can add, delete or update the tracker according to his/her will.

**Technologies used :**
1. *<u>Bootstrap</u>*- designing the look/aesthetics of the application.
2. *<u>Flask</u>*- developing web applications using python.
3. *<u>Flask-sqlalchemy</u>*- used to create database schema and tables using SQLAlchemy with Flask by providing defaults and helpers.
4. *<u>Datetime</u>*- a python module which supplies classes to work with date and time. Here, datetime module to create timestamp in the application.
5. *<u>matplotlib.pyplot</u>*- a python module is used to create dynamic trendline graphs based on the information provided by the user.
6. *<u>render_template</u>*- used to render html templates based on the Jinja2 engine that is found in the application's templates folder.
7. *<u>request</u>*- used to handle HTTP requests and responses.
8. *<u>flash</u>*- used to generate informative messages in the flask.
9. *<u>redirect-</u>* used to redirect a user to another endpoint using a specified URL and assign a specified status code.
10. *<u>session-</u>* Flask extension supports Server-side session to our application.
11. *<u>before_first_request-</u>* helps us to execute the code at least once before a user arrives, before the first request arrives
12. *<u>route-</u>* used to bind the specific URL with the associated function that is intended to perform some tasks.

***Database Schema :***

1. *<u>Relation-</u>* A user can have several trackers and thus we have one-to-many relationship between User_Profile and Tracker. Two secondary tables- user_trackers and trackers_logs is used to establish one-to-many relationship with User_profile,Tracker and logs.

2. *<u>ER Diagram</u>* - [ER Diagram Link](https://drive.google.com/file/d/1gMMSsRCffGzfzePtIJujhxNgMT-kNyog/view?usp=sharing)

<br>

***Architecture and Features:***

The project code is organised based on its utility in different files. I have named my project Self Tracker. Inside this folder there is a python files app.py; sqlite database page; static folder containing all the required images for the application, a folder named templates that contains all the HTML (Jinja) files, Report folder with the report.pdf file that is short description of application and Db_setup folder containing a python file module.py - used to develop the databases – User for user details, Tracker for tracker details and Logs for log details of the tracker along with 2 secondary tables to connect the databases. The HTML file includes the login, sign up, dashboard, landing and all other pages required to update, add and delete the tracker details along with a page for each kind of tracker- Numerical and Boolean. The main page contains all the controllers used to access the model and modify the view of the app.

***Flowchart of Tracker App:*** [link to flowchart](https://drive.google.com/file/d/1b2KmZqacQxGXzwggaUoIBf8AW8xTh2DK/view?usp=sharing)

- @app.before_first_request
- @app.route('/', methods=["GET"])
- @app.route('/about_us', methods=["GET"])
- @app.route('/contact', methods=["GET"])
- @app.route("/login", methods=["GET", "POST"])
- @app.route("/sign_up", methods=["GET", "POST"])
- @app.route("/< string:username>/dashboard",  methods=["GET"])
- @app.route("/logout",  methods=["GET"])
- @app.route("/< string:username>/create_tracker",methods=["GET", "POST"])
- @app.route("/< string:username>/update/< int:id>", methods=["GET", "POST"])
- @app.route('/< string:username>/< int:id>/delete', methods=["GET","POST"])
- @app.route("/< string:username>/< int:id>/logs",methods=["GET", "POST"])
- @app.route('/< string:username>/< int:tracker_id>/< int:log_id>/delete', methods=["GET"]) 
- @app.route("/< string:username>/< int:tracker_id>/< int:log_id>/update", methods=["GET","POST"])


***Video link:*** [Video Link](https://drive.google.com/file/d/12MdkSoQg_NjUYLBQL2-v6HsCdpp1HjnC/view?usp=sharing)