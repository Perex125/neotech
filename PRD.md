
# ResponsePoint

## Overview

For awhile now students have been complaining about how difficult, slow and stressful it is to report issues to higher authorities, and many give up before anyone hears them. 

The process is also very stressful and time consuming. Students may have to visit different offices, wait for hours before meeting someone, or struggle to find the right person to address their problems. Sometimes, they are sent from one office to another without getting a clear answer.  
As a result, many students choose to remain silent even when they have problems that need attention. Some issues remain unsolved simply because students do not know how to tell them or do not feel comfortable approaching the appropriate authorities.

That's why we have come up with an application that solve that particular issue, Introducing **ResponsePoint**  an application built on the concept that speaking up shouldn't be hard, this application makes student feel attended to, when they report a problem or make enquiries about something on campus. 
It is built with the idea of speed, convenience, availability and attentiveness in mind so that every complaint is swift, and easy for every staffs to respond to and convenient for student to get attended to.

*Reach out once. Get heard.*

- **What it is:** a web app with two sides: students report and track, staff receive and resolve.
- **Who it's for:** students in Babcock University, and the staff who look after them.
- **How it can be accessed:** any device with a web browser can access it, nothing to download.
- **The promise:** every report gets a tracking code, and every code shows a clear status.
- **Where we are:** defining the MVP, which starts with hall faults and is built to grow into a wider way for students to raise complaints with university authorities.

## Vision and goals

**Vision:** a university where getting solutions to issues is easy, and where every student knows what happens next.

**Goals**

- **For students:** report a fault without queues, office-hopping or awkward conversations, and always know where it stands.
- **For staff:** receive reports that already say which student and what kind of issue they are having, and keep their status honest and current.
- **For the university:** see patterns (which fault types, which student, how long things stay open) and use them to decide where to act.

## Who it's for

ResponsePoint has two groups of users, and the app is built as two sections to match.

| User    | What they need                                                                                                                                                  | What they worry about                                                                                        |
| ------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Student | A quick, simple way to report a fault/issue, and proof it was received                                                                                          | Wasting time, being sent from office to office, being ignored, feeling uncomfortable approaching authorities |
| Staff   | A clear list of reports by hall and type of issue(either academic or domestic/hall related), with unsafe issues easy to spot, and a simple way to update status | Reports getting lost, unclear ownership, extra admin work to organize the list of issues                     |

Students come with very different levels of comfort with technology. ResponsePoint is a web app because everyone has used one before, it runs on any device that has a browser, and you don't needs no install anything.

## MVP scope

The MVP is the smallest version of ResponsePoint that shows whether students will report faults this way and whether staff will keep statuses current.

**In the MVP**

- Two sections, a student version and a staff version, with the visuals designed for both.
- A report form: hall, room, fault type, short description, an optional photo, and an "unsafe" checkbox.
- A tracking code and a status page where the student enters the code to see where their report stands.
- Four statuses: Reported, Seen, In progress and Resolved.
- A notification section in the staff version.

**Not in the MVP** *(to be added in the later version)*

- Automatic routing of reports to named officers.
- Complaint categories beyond hall faults. These come once the MVP shows the model works.
- Appointments if the issue can't be solved without the person being there 

## Functional requirements

Every requirement below belongs to the MVP. Together they let a student report an issue and follow it till resolved, and let staff act on it.

**Student side**

| ID  | Requirement                                                                                                                     | Notes                                               |
| --- | ------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| S1  | Submit a report by choosing a hall, entering a room number, matric number, picking a fault type and writing a short description | All five fields are required                        |
| S2  | Attach a photo to a report                                                                                                      | Optional                                            |
| S3  | Mark a report as unsafe, yes or no                                                                                              | Lets staff see urgent issues first                  |
| S4  | Receive a unique tracking code once the report is submitted                                                                     | Shown clearly on screen and, easy to copy and paste |
| S5  | Enter a tracking code on a status page and see the report's current status                                                      | No account needed to check, as proposed             |

**Staff side**

| ID  | Requirement                                                                                                            | Notes                                                        |
| --- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| T1  | See all incoming reports with hall, student matric number, room number, fault type, description, photo and unsafe flag | Helps staffs prioritize which issue needs to be solved first |
| T2  | Be notified of new reports in a notification section                                                                   | Unsafe reports should stand out                              |
| T3  | Change a report's status to Seen, In progress or Resolved                                                              | New reports start as Reported                                |


**Statuses**

| Status      | Meaning                                       |
| ----------- | --------------------------------------------- |
| Reported    | The report has been received                  |
| Seen        | A staff member has opened and acknowledged it |
| In progress | Someone is working on the fix                 |
| Resolved    | The fault has been fixed                      |

## Non-functional requirements

Hallo has to feel easy for every student, so these qualities matter as much as the features. Targets are starting points to tune after testing.

- **Ease of use:** a student with no technical background can file a report without help. Plain language, few fields, one clear action per screen.
- **Any device:** works in any machine that has a web browser weither on phones, tablets and computers, with nothing to install.
- **Light and fast:** pages stay small and the photo is optional, so reporting still works on a weak connection.
- **Privacy:** a report is visible only to the student holding its tracking code and to authorised staff. Students are told plainly who can see what they submit.
- **Security:** the staff  and student sections are behind a login, and stored data and photos are protected.
- **Reliability:** a submitted report is never lost, and a status change shows up on the status page straight away.
- **Accessibility:** readable text, good contrast and big tap targets even your grandmother can use it.

## Data and technical approach

ResponsePoint is a web app built with familiar tools: students already know how to use a browser, and the browser brings many features built in.

| Layer            | Technologies             | Role                                                  |
| ---------------- | ------------------------ | ----------------------------------------------------- |
| Frontend         | HTML, CSS and JavaScript | The student and staff screens that they interact with |
| Backend          | Node.js                  | Application logic behind both sections                |
| Database linking | PHP                      | Connects the application to the database              |
| Database         | MySQL                    | Stores reports, logins and their history              |

The MVP features also imply a short description, an optional photo, the unsafe flag, the tracking code, the current status and timestamps. The timestamps are what make "average days open" possible.

The application uses both Node.js and PHP for the backend and database linking.

## Resources needed

Building ResponsePoint takes more than code. It needs five kinds of support.

- **People:** developers and software engineers to build it, students to test it, and university officials to manage it and act on what comes in.
- **Technology:** servers, internet access, software's and a database to store reports and responses.
- **Money:** funds for hosting, internet, maintenance and upgrades in the future.
- **University support:** cooperation from school authorities so reports reach the right people and get addressed. Without this the app is a mailbox nobody opens.
- **Research:** student feedback, interviews and surveys, so ResponsePoint is built around the issues students actually face.
