# Team-7-MIST-4610-Group-Project-1

# Team Name
47114 Group 7

## Team Members:
1. Leif Hurdal ([@leifhurdal](https://github.com/leifhurdal))
2. Amy Morales ([@amymorales](https://github.com/amyfrmorales))
3. Dung Nguyen ([@dungnguyen](https://github.com/den50791))
4. Vivian Pham ([@vivianpham](https://github.com/vivianxpham))
5. Ben Williams ([@benwilliams](https://github.com/bendeanwilly))

# Problem Description 


## Data Model

<img width="813" alt="Screenshot 2024-03-26 at 1 53 54 AM" src="https://github.com/den50791/MIST-4610-Group-7/assets/163002845/27c21c52-29b9-4582-98ed-cb1811c1911e">

Explanation of data model:

Our data model seeks to organize the above-described emergency clinic. The core of the model is the Appointment entity, which is the instance in which a Patient meets with a Healthcare Provider. The Appointment entity includes information about where and when the Appointment takes place. Five relational branches stem from an appointment.

The first branch that comes from the Appointment is Patient. Each Patient can book many Appointments over the course of their life, hence the one-to-many relationship between them. As the name suggests, the Patient table includes critical information about each Patient, including a Unique Identifying ID, Name, Number, Gender, and Date of Birth.
The Patient table itself has two additional relationships with other entities. Each Patient will have a unique Medical History associated with him/her (one-to-one relationship). This history will include Immunization, Medical Conditions, Medications, etc. The other branch for Patient is Prescription. At the clinic, each Patient can receive many Prescriptions (one-to-many relationship). 

Additionally, each Prescription comprises many Medications, and many different Prescriptions will use the same kind of Medication. Prescription and Medication are joined using the associative entity of Prescription Order. Prescription includes information on the Name, Frequency, and Issue Date of the Prescription. Medication consists of the Name, Type, and Description of the medication. PrescriptionOrder includes the amount and refills of each Medication.

The second branch, which comes from Appointment, is Healthcare Provider. Similarly to the previous relationship, one Healthcare Provider will have many Appointments over their career (helping Patients), leading to another one-to-many relationship. The Healthcare Provider table provides information on them such as Name, Specialization, Schedule, etc.

The third branch is Billing. At the end of each Appointment there will be one bill to pay, hence the one-to-one relationship between Billing and Appointment. The Billing table has information to keep track of the payment such as Date, Amount, etc.

The fourth Branch is Appointment Type. Each Appointment - of the many Appointments that take place - will be classified by an Appointment Type. This relationship will mean there is a one Appointment Type that classifies many Appointments (one-to-many relationship). Having a categorization for Appointments will provide additional organization for the clinic. The Appointment Type entity includes the appointment type Name, Detail and Service Hours.

The fifth and final branch off of Appointment is Diagnostic Tests. During an Appointment there can be many Diagnostic Tests facilitated by a Healthcare Provider. This means there is a one-to-many relationship between them. The Diagnostic Test table includes information such as the name of the test, the description of it, and the result.
	
Each Diagnostic Test requires many pieces of Equipment can be used and each piece of Equipment can be used in many different kinds of Diagnostic Tests. These two are connected by the associative table of EquipmentUsed which includes the condition and quantity of the Equipment. The Equipment table stores the Name, Type, Condition, and Maintenance History.
   
## Data Dictionary 

<img width="636" alt="Screenshot 2024-03-26 at 1 56 46 AM" src="https://github.com/den50791/MIST-4610-Group-7/assets/163002845/254aec45-792e-4790-977a-8fd616705fa7">

<img width="622" alt="Screenshot 2024-03-26 at 1 51 09 AM" src="https://github.com/den50791/MIST-4610-Group-7/assets/163002845/e0329170-9fb4-4ced-a6cd-588f467aa7a2">

<img width="639" alt="Screenshot 2024-03-26 at 1 59 41 AM" src="https://github.com/den50791/MIST-4610-Group-7/assets/163002845/ec95f299-e9ab-4422-a0c3-b4374bd653a2">

<img width="634" alt="Screenshot 2024-03-26 at 2 00 50 AM" src="https://github.com/den50791/MIST-4610-Group-7/assets/163002845/b61ed417-b9d8-4319-ba65-65853a739007">

<img width="633" alt="Screenshot 2024-03-26 at 2 02 01 AM" src="https://github.com/den50791/MIST-4610-Group-7/assets/163002845/7c53f475-a352-47b3-aaf1-6de36ce6a11c">

<img width="625" alt="Screenshot 2024-03-26 at 2 02 41 AM" src="https://github.com/den50791/MIST-4610-Group-7/assets/163002845/d5ecb799-fece-4896-865f-4bc5d08a1f55">

<img width="629" alt="Screenshot 2024-03-26 at 2 03 32 AM" src="https://github.com/den50791/MIST-4610-Group-7/assets/163002845/08f44614-90f0-4fd4-894d-50422538a960">

## Queries


## Database Information
