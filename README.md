# Medical-Appointment-No-Shows
Sourced from : https://www.kaggle.com/datasets/joniarroba/noshowappointments

Cleaning Process:

1. Age cannot be less than 0 considering 0 is the age of an new born found age in negative this is an anomaly thus used delete sheet rows to remove the row containing the anomaly
2. PatientID column contained numbervalues as well as Scientificvalues which was decided to be standardized to numbervalues using the following steps Click on the Row Name to select the entire row > Right click > Select Format cells > Select Numbers
3. ScheduleDay column contained Date and Time in the ISO format used =SUBSTITUTE(LEFT(D2, LEN(D2)-1), "T", " ") function to create a new column ScheduleDateTime to convert it into standard format
4. AppointmentDay column contained Date and Time in the ISO format used =SUBSTITUTE(LEFT(F2, LEN(F2)-1), "T", " ") function to create a new column AppointmentDateTime to convert it into standard format

scholarship variable means this concept = https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia

Variables:

01 - PatientId : Identification of a patient
02 - AppointmentID :Identification of each appointment
03 - Gender : Male or Female . Female is the greater proportion, woman takes way more care of they health in comparison to man.
04 - ScheduleDay : The day of the actuall appointment, when they have to visit the doctor.
05 - SheduleDateTime : The day of the actuall appointment in standard format.
06 - AppointmentDay : The day someone called or registered the appointment, this is before appointment of course.
07 - AppointmentDateTime : The day someone called or registered the appointment in standard format
08 - Age : How old is the patient.
09 - Neighbourhood : Where the appointment takes place.
10 - Scholarship : True of False . Observation, this is a broad topic, consider reading this article https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia
11 - Hipertension : True or False
12 - Diabetes : True or False
13 - Alcoholism : True or False
14 - Handicap : True or False
15 - SMS_received : True or False.
16 - No-show : True or False.
