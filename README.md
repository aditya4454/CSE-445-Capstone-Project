# CapStone Project(CSE-445)

## Introduction
> 1. This project takes student attendance using facial recognition. <br>
> 2. The admin is authentic person who can create an account . <br>
> 3. The admin can register new student by taking their personal information following that student dataset is generated and stored in database <br>
> 4. After this process admin can take student's attendance using this system <br>
> 5. Inside this project there is indivisual account of student where student can check their attendance report also.<br> 

## Tech Stack

**Client:** HTML, CSS, Javascript

**Server:** Python, Django

**Database:** sqllite


## Setup Instructions

### For Local Device

```bash
pip install -r requirements.txt
```

Next run the django web server.
```bash
python manage.py runserver
```

Go to Local host
```bash
http://127.0.0.1:8000/
```

### Deployed 
```bash
Yet to be done!!
```

## Modules

### Home
>  Home page is predominantly the page from where the control of the system follows. It consist of various sub modules such as :-

![Screenshot (142)](https://user-images.githubusercontent.com/62827632/169697714-9de9fd3d-85d0-4d6a-af3c-1600d552893f.png)
#### Mark Your Attendance In :-
> As the name suggest😀 this module verify and tracks the time at which Student has marked the attendance in. The way this module work is based on computer vision and machine learning, we already have the model which is trained on the images stored in the DB. Using computer vision we get the face of the Student and then using our model it verify whether the student match with the data in DB and is so what's his/her name.

![Screenshot (152)](https://user-images.githubusercontent.com/62827632/169698202-4d66dd0f-1289-4348-a855-08ed4314a038.png)


#### Mark Your Attendance Out :-
> This module is just vice-versa of the above discussed module😛. The only difference is that instead of marking the time in, it marks it out.

![Screenshot (153)](https://user-images.githubusercontent.com/62827632/169698210-03dae9db-23cb-4323-a51a-22bf98c9b1c4.png)

### Log In
> There are two portal based on the login credentials enter. Those are :- 
> 1.) Admin Panel :- If the user is admin it will redirect to Admin Dashboard
> 2.) Student Panel :- If the user is Student it will redirect to Student Dashboard.

![Screenshot (143)](https://user-images.githubusercontent.com/62827632/169697792-b5c023d8-56e7-4988-99e4-13d7da81be89.png)

### Admin Dashboard
> The admin dashboard looks like :- 

![Screenshot (149)](https://user-images.githubusercontent.com/62827632/169697820-1493a416-3405-4e4d-8e6f-7ca15d0e4730.png)

>  It has following Following Submodules :- 
#### Register New Student :- 
> This module register a new student.

![Screenshot (145)](https://user-images.githubusercontent.com/62827632/169697836-f30d40ae-5763-4f73-93a3-9247c2c36191.png)

#### Add Photos :- 
> This module takes the name of the register student and open a camera window using computer vision and store them in DB (Currently there's scope of taking 25 photos only 🙃🙃 ).

![Screenshot (146)](https://user-images.githubusercontent.com/62827632/169697854-74717908-305d-41fb-934e-c23f05ed6efb.png)

#### Train :- 
> The stored image dataset is then picked and trained using SVM classifier (as it's a classification problem😁) 

![Screenshot (150)](https://user-images.githubusercontent.com/62827632/169697875-6f583c05-63bf-4f88-8834-119d529cc8ba.png)

#### View Attendance Reports :-
> This module contains graphs and details of Attendance related to all the student, admin can see the details of a particular student, date wise and range wise details, etc.

![Screenshot (154)](https://user-images.githubusercontent.com/62827632/169698219-15799e1d-5ac6-4041-bc45-c42490fff9eb.png)

### Student Dashboard 
> This module has graphs and details of Attendance related to a Student  

![Screenshot (148)](https://user-images.githubusercontent.com/62827632/169697882-712578df-b5a8-44a7-8d5c-4ea85ad84093.png)

## Authors

- [@Aditya Senger](https://github.com/aditya4454)
- [@Naveen Kumar Yadav](https://github.com/montyydv)
- [@Mrityunjay mishra](https://github.com/Mrityu2802)
- [@Vikas Malviya](https://github.com/VikasMalviya2111)
