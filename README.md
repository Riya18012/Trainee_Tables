# Trainee_Tables
All related entities of Trainee management system
Entities:
1.	Trainee
2.	Courses
3.	trainer
4.	Batch
5.	Enrolments
6.	Payment
7.	Certificate


Attributes:
1.	Trainee: 
1.	Trainee_id            {primary key}
2.	Name
3.	Age
4.	Gender
5.	Contact number
6.	Email
7.	Address           fk
8.	Nationality
9.	Date of birth
10.	College/school


2.	Courses:
a.	course_id    pk
b.	course_name
c.	description
d.	Duration
e.	StartDate
f.	EndDate
g.	TrainerID    fk
h.	Status     The status of course (e.g., upcoming, ongoing, completed, canceled).
i.	fee

 
4.	Trainer
1.	TrainerID  pk
2.	Name:
3.	Age
4.	Gender
5.	Contact number
6.	Email
7.	Address          
8.	Designation

   
4.	Batch:
1.	BatchID pk
2.	CourseID  fk 
3.	TrainerID     fk
4.	StartDate
5.	EndDate
6.	Location:
7.	Capacity
8.	EnrolledTrainees:
9.	Status   The status of the batch (e.g., upcoming, ongoing, completed, cancelled).


5.	Enrolments:
1.	EnrollmentID   pk
2.	TraineeID    fk
3.	BatchID    fk
4.	EnrollmentDate
5.	Status  The status of the enrollment (e.g., enrolled, completed, dropped, pending).
6.	Payment status
7.	Payment date
8.	CertificateIssued (true or false)
9.	CertificateID:    fk


6.	Payment:
1.	Paymentid     pk
2.	Traineeid     fk
3.	Batched         fk
4.	Payment date
5.	Payment amount
6.	Payment method
7.	Payment status


7.	certificate
1.	CertificateID pk
2.	TraineeID   fk
3.	BatchID fk
4.	CourseID fk
5.	IssueDate
6.	IssuedBy
