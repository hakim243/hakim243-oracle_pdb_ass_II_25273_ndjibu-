📌 ASSIGMNET OVERVIEW

This assignment focuses on understanding and applying Oracle Multitenant Architecture concepts. The work involved creating, managing, verifying, and deleting Pluggable Databases (PDBs), as well as configuring database administration tools.

The assignment helped me gain practical experience in Oracle database container management and user administration.


ENVIRONMENT USED 

Oracle Database 21c Enterprise Edition
SQL*Plus Command Line Tool
Oracle Enterprise Manager Express
Windows Operating System





Task 1 – Create a New Pluggable Database
Objective

Create a new Pluggable Database using the required naming convention and create a user inside it for future class work.

Step 1: Viewing Existing PDBs

I first checked existing pluggable databases using:

COMMAND: SHOW PDBS
This allowed me to confirm the database environment before creating a new PDB.
<img width="1365" height="767" alt="Screenshot 2026-02-17 090530" src="https://github.com/user-attachments/assets/1a6d18df-e0c3-4d27-abb1-2752d4344d76" />



Step 2: CREATING THE PDB

I created the new pluggable database using the required naming convention:

NAMING CONVENTION:   NDJ_PDB_25273

<img width="1365" height="767" alt="Screenshot 2026-02-16 152958" src="https://github.com/user-attachments/assets/8d35f41f-37b2-46fe-a60d-0893e192b64d" />
The database was successfully created and verified.

Step 3: OPENING THE PDB

The PDB was opened using:
COMMAND: ALTER PLUGGABLE DATABASE NDJ_PDB_25273 OPEN;
<img width="1338" height="767" alt="Screenshot 2026-02-17 090951" src="https://github.com/user-attachments/assets/0d5b754e-7a3f-4eb0-971b-6545b8e71bd2" />

The database is already opened as the screenshort shows and it's in read write mode 



Step 4: CREATING USER INSIDE PDB

I switched to the PDB container and created the required user:
ndjibu_plsqlauca_25273

Privileges granted:

CONNECT
RESOURCE
This user will be used for future practical coursework.
<img width="1365" height="767" alt="Screenshot 2026-02-16 153447" src="https://github.com/user-attachments/assets/614defad-eb50-4327-84ae-e625511f645c" />


Task 2 – Create and Delete a Temporary PDB
Objective

Demonstrate understanding of the PDB lifecycle by creating and deleting a temporary pluggable database.

Step 1: CREATING TEMPORARY PDB 

The temporary database created was:
ND_TO_DELETE_PDB_25273
<img width="1365" height="767" alt="Screenshot 2026-02-16 153512" src="https://github.com/user-attachments/assets/d9430e64-5767-48e7-af19-0a61f4efeebe" />
The database appeared in MOUNTED state.

Step 2: ATTEMPTING TO CLOSE TEMPOPARY PDB

While closing the PDB, the system returned:
<img width="1188" height="451" alt="Screenshot 2026-02-17 091441" src="https://github.com/user-attachments/assets/77a36bf6-5413-4283-ab3a-39a911153c1f" />

Step 3: DELETING TEMPORARY PDB

The temporary PDB was deleted using:
COMMAND: DROP PLUGGABLE DATABASE ND_TO_DELETE_PDB_25273 INCLUDING DATAFILES;

<img width="1365" height="767" alt="Screenshot 2026-02-16 153623" src="https://github.com/user-attachments/assets/06d9facd-2e8a-404e-99cf-638317ee3781" />

Task 3 – Oracle Enterprise Manager (OEM)
IT'S HERE I REAALY GOT STUP EVEN THOUGH I TRIED LOGIN MY REAL CREDENTIALS BUT I COULD STILL LOGIN INTO OEM BUT ACCESSING IT YES I HAVE ACCESSED IT:
<img width="1364" height="766" alt="Screenshot 2026-02-16 172444" src="https://github.com/user-attachments/assets/2f05012e-7ab1-4296-ab18-b242aeea11d5" />


CHALLENGED FACED 

During this assignment, I experienced several technical challenges including:

1. Listener Connection Errors

The database initially failed to connect due to service registration issues.

2. Authentication Problems

Login failures occurred due to incorrect credentials and role requirements.

3. OEM Access Issues

Oracle Enterprise Manager required correct port configuration and container selection.


EVIDENCE PROVIDED 

Screenshots and command outputs included in this repository demonstrate:

Creation of main PDB
<img width="1365" height="767" alt="Screenshot 2026-02-16 152958" src="https://github.com/user-attachments/assets/4b73c659-0637-4f84-8623-3429561650f3" />

User creation and privilege assignment
<img width="1365" height="767" alt="Screenshot 2026-02-16 153424" src="https://github.com/user-attachments/assets/6e548d71-a529-4313-8328-69ea14ae8787" />

Temporary PDB creation and deletion
<img width="1365" height="767" alt="Screenshot 2026-02-16 153605" src="https://github.com/user-attachments/assets/d47e0817-5098-4cce-ac69-aea3d433c3d7" />

Verification of database states
<img width="1365" height="767" alt="Screenshot 2026-02-16 153623" src="https://github.com/user-attachments/assets/b72f8142-d07f-403d-a47a-f395c1e79b0f" />

OEM configuration attempts
<img width="1364" height="766" alt="Screenshot 2026-02-16 172444" src="https://github.com/user-attachments/assets/c3f2493a-dd82-49ca-a27b-202247584178" />




LEARNING OUTCOME

This assignment strengthened my understanding of:
Oracle Multitenant Architecture
Container and Pluggable Database management
Database user administration
Oracle system troubleshooting


CONCLUTION 

The assignment provided valuable hands-on experience in Oracle database administration. It improved my confidence in managing pluggable databases and handling real-world database configuration issues.

INTERGRITY STATEMENT 

I confirm that this assignment was completed individually. All commands, screenshots, and documentation reflect my own practical work and understanding.
