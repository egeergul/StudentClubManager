# student-club-manager

## This is the repository of CS319 term project.
-----------------------------------

## IMPORTANT:
1) We have developed frontend in another repository. Frontend original repository's link: https://github.com/egeergul/ohmygoat
2) We have implemented a sample database, you can find this example data in the file called db_export.sql. The passwords of users in this sample db are 123456
3) In the frontend repository, all the commits of @emreerdal9 are done by @keremerdal

### Developers (GOATs):

* Emre Erdal 21901597
* Kerem Erdal 21901596
* Beste Güney 21901631
* Efe Ertürk 21902620
* Ege Ergül 21902240
* Doruk Onur Çalışkan 21902672

-----------------------------------

# Build Instructions
## Prerequisites
* Install MySQL Server and Workbench v-8.0 and above
* Java JDK v-8 and above
* Maven v-3.6.3 and above
* Node.js v-15.6.0 and above
## Installation
* Go to GitHub Link: https://github.com/Beste-Guney/student-club-manager
* Download the zip file of the project and open it with preferably IntelliJ Ultimate
on your local device
## Database Setup
* Open MySQL Workbench and from Management section choose data import
* Choose import from self-contained file
* Choose the demo database we have provided you ( db_export.sql). You can
find this file in the zip folder you have downloaded.
* Choose the default target schema. Do not forget the schema name as you will
be needing it later on
* Choose dump with structures and data
* Click to start the import
* When it is done, your tables should be downloaded to the database.
## Running
* In IntelliJ, go to src/main/resources/application.properties. In this file, choose
the correct database name for the connection which you should have already
set up in the previous step.

## Note: we assume that your MySQL server runs at port 3306. If it is not, you
should edit as well.
Figure 44: IntelliJ screen for setting up database environment
* At IntelliJ Ultimate, open a terminal and go to the frontend directory
* Run the following command: npm install
* Run the backend spring project ( by the run button on the uppermost right
corner)
* When the installation and running of the backend project is done, return to the
terminal and run the following command: npm start
## Check Provided Data
* Once the project is up and running on localhost:3000, you can use the
following credentials for logging in or you can sign up by yourself as a student.
* For Student Login:
username: user1
password: 123456
For Advisor Login:
username: advisor1
password: 123456
* For Admin Login:
username: admin
password: 123456
## Important Note: One cannot signup as an admin or advisor. For admin login,
you have to use the provided admin credentials and advisors will be signed up
by the admin.
Also, there exists 3 users (user1,user2,user3) with the same
passwords(123456), 3 advisors (advisor1,advisor2,advisor3) with the same
passwords(123456). You can login by using these credentials.
You can check the rest of the existing data by the database. For simplicity,
you can inspect the database from IntelliJ.

-------------------------------

# Plans for the project:

There will be two main actors in the system: Clubs and Students.

#### Club System:

* There will be a club registeration. For already existing clubs, they will be able to register the club for the first
  time and also if a new club opens they also will be able to register their club to the system. While registering for
  the first time, the system will require a password and a name.
* Clubs will have a profile. In this profile, they will have url links to whatsapp, instagram, twitter, mail and etc. In
  addition to that, their activity calendar will be on this profile. Clubs will have forums inside their profile. Inside
  this profile members of the clubs will be seen.
* Clubs will be able to create and post new events. Each event will have a forum and participants list. After the event,
  clubs can upload media like pictures or videos to the event detail.
* There will be a notification menu for clubs and each reported forum message will be shown here. Also forum posts will
  be notified.
* Clubs will hold the participants and their related GE250 information for events.
* Club will have a page in which they will hold club records and folders. For example, when board members have a meeting
  document they will be able to upload there.

#### Student System:

* Can list existing clubs
* Can register or unregister to an existing club
* Can view all upcoming club events as a calendar. Also they can filter which clubs to see.
* Can register to an upcoming event or unregister
* Activiy calendar for students to follow their activities. If they are a member already, that club's activities will be
  placed on calendar.
* Can discuss and comment on the upcoming club events on a forum
* Can report comments on a forum
* Students will be notified by clubs forum posts and system will automatically notify them when a registered event is
  upcoming.
* They can edit their profiles, add interests, pictures etc.
