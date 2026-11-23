
2026-11-22 13:37

Tags: #assignment #web-dev
### Resources


# Main Note

For awhile now students have been complaining about how difficult and stressful it is to repot issues to higher authorities.  
The process can also be very stressful and time consuming. Students may have to visit different offices, wait for hours before meeting someone, or struggle to find the right person to address their problems. Sometimes, they are sent from one office to another without getting a clear answer.  
As a result, many students choose to remain silent even when they have problems that need attention. Some issues remain unsolved simply because students do not know how to tell them or do not feel comfortable approaching the appropriate authorities.


**Resources Needed to Solve the Problem**  
  
To develop an application/software that allows students to report complaints to the university authorities, the following resources are needed:  
  
• People: Developers, Software Engineers, students, and university officials to build, test, and manage the app.  
• Technology: Servers, internet access, software, and a database to store complaints and responses. 
• Money: Funds for hosting, internet, maintenance, and possible future upgrades.  
• University support: Cooperation from school authorities to ensure complaints reach the right people and are addressed.  
• Research: Student feedback, interviews, and surveys to understand the problems students face.  

These resources will help us build a platform where students can speak up, report problems, and receive feedback from the appropriate authorities.

**Developing The MVP**

To develop this Application to be easily useable by all students of different technological background we have decided to make it a webapp since everyone has interacted with a webapp at least once in their life and it has different technologies already built into the browser and it can be run on any device with a web browser. 

As for the programming languages that would be used in the development of this application, we are going to be using the following:
- HTML, CSS & JavaScript for the frontend of the webapp
- Node JS as the framework for the backend
- PHP for the linking of the database to the application
- MySQL database for the saving of information such as complaints, Room number, Matric number, hall of resident, the type of complaint etc.


**Documentation of the MVP**

The MVP is the smallest version that shows whether students will report faults this way and whether staff will keep the status current.

- First we have to consider that we are working with 2 different sections of the app (The student version and the Staffs version) then we develop the visuals of both section of the application.
- A report form: hall, room, fault type, short description, optional photo, and an "unsafe" yes or no.
- A tracking code and a status page where the student enters the code to see status (such as received).
- Statuses: Reported, Seen, In progress and Resolved.
- A Notification Section on the staffs version
- A basic summary for the team: reports per hall, per type and average days open.