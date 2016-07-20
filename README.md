# Message My Driver

### To-do:
 - [x] Create DB
 - [x] Create Tables
 - [ ] Style Homepage
 - [ ] Add viewing of specific license plate
 - [ ] Add report submitting


### DB Layout:

#### Cars
- id - PRIMARY int AUTO_INCREMENT
- uid - varchar(20) UID
- license - varchar(8)
- state - varchar(2)
- date - timestamp CURRENT_TIMESTAMP

#### Reports
 - id - PRIMARY int AUTO_INCREMENT
 - uid - varchar(20) UID
 - carid - int
 - user - int
 - report - text
 - date - timestamp CURRENT_TIMESTAMP

#### Users
 - id - PRIMARY int AUTO_INCREMENT
 - uid - varchar(20) UID
 - passkey - varchar(40)
 - email - varchar(256)
 - datejoined - timestamp CURRENT_TIMESTAMP

#### Subscriptions
 - id - PRIMARY int AUTO_INCREMENT
 - userid - int
 - carid - int
