README FOR student-management-api

## About
This is a student management REST-API which was built using python Flask and Flask-smorest.
The application can be used for the following:

##Features
- Register students into the school's system
- Create new users to manage the application
- Administrators and users can add or register students. Student ID and password will be automatically generated once they are registered
- Students can login with Student ID and password provided upon registeration
- Administrators of the application can add a new course to which students can later login to enroll for the course of thier choice
- Administrators and users of the application can add scores for students based on the courses they are enrolled under. 
- This application automatically calculates the grades and GPA of students once a student is registered and enrolls for a course or courses
- All courses should have a code which students will use to enroll. E.g A Computer Science course can have a course code as CS001
- Once logged in, a student can view all available courses to enroll for, he or she can view all the course enrolled under as well as the grades for each course
- Students can also view thier basic details or information, request for a password change if forgotten, and also be able to change thier passwords.
- All other routes except enrolling for a course can be accessed by an Administrator.
- However, a user who is not an administrator has some restrictions like updating and deleting a student or course.
- This application also enables the user to retrieve all students and all courses. One can also view a student by his or her ID and also view a course by its code
- You can also view all the students enrolled for a particular course as well as all the courses a particular student has enrolled for
- All the grades of each student for a particular course can also be retrieved. A student can also retrieve all the grades for all the courses they have enrolled for
- Students can view thier GPA and users and administrators can view the GPA of all students

#Usage
You try this application, you can either clone and run it locally on your PC or visit (this-site) to check it out.
Follow the steps below to run and test the application locally

##How to run the app locally
1. Clone this app
```
git clone ..........................
``` 
2. CD to the root directorate of the project and install create your virtual environment
```
cd student-management-api
``` 
```
python -m venv env_name
``` 
3. Activate your virtual environment
```
source env_name/Scripts/activate #for windows
``` 
```
source env_name/bin/activate #for linus and MacOS
``` 
4. Install all packages from the requirements.txt file
```
source env_name/Scripts/activate #for windows
``` 
5. Run the application to get started
```
flask run
``` 
or 
```
python run.py
``` 

# Once the application is running, you can start testing it with the following admin credentials
- username: superadmin
- password: password

- Login as an admin to get a JWT token. Once you add the token to authorization header to can go ahead and create a new user or student.
- You can also view students already added in the system. All other routes can b tested once you are logged in as an admin
- If you need to perform as task as a student (eg. enroll for a course) you'll need to login as a student to do that.
- You can go ahead and create a new student to get the student ID and password. You may also use an already registered student details for testing
- student_id: ATS00002
- password: AGOulsYB

You can visit (this-site) as well to test the already hosted application with the same credentials provided above.

#ENDPOINTS



## Languages and Tools Used
- Python
- Flask
- SQLAlchemy
- SQLite
- Flask Smoorest

