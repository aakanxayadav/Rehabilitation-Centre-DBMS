# Rehabilitation-Centre-DBMS

This repository contains a database schema and sample data for a rehab center. The database is designed to manage patient information, treatment plans, and other relevant details within a rehabilitation facility. This database will also help us to find out useful insights about rehab society. The data used in project is created fictionally.

## Database Overview

- **Database Name:** patients
- **Tables:**
  - patient basic information
  - therapists
  - treatments
  - insurance provider
  - emergency contact
    


## Sample Queries

Here are some sample SQL queries you can run on the database:

1. Retrieve all patient information:

    ```sql
    SELECT * FROM patients;
    ```

2. Find therapists and their assigned patients:

    ```sql
    SELECT therapists.*, patients.*
    FROM therapists
    JOIN patients ON therapists.TherapistID = patients.AssignedTherapistID;
    ```

3. Update patient details:

    ```sql
    UPDATE patients
    SET ContactEmail = 'newemail@example.com'
    WHERE PatientID = 101;
    ```

## Instructions

1. **Database Setup:**
   - Execute `patients.sql` to create the database schema.
   - Execute `patients_data.sql` to populate the database with sample data.

2. **Explore the Data:**
   - Run your SQL queries to explore and analyze the rehab center data.
   - Use the provided sample queries as a starting point.

3. **Contribute:**
   - If you have improvements or additional features, feel free to contribute by submitting a pull request.

## Disclaimer

This is a fictional database created for educational purposes. Any resemblance to real persons or entities is purely coincidental.
