[Return to Panagiotis Bernalis' GitHub Profile for more innovative projects](https://github.com/pbernalis)

# Hospital Information System Oracle APEX

A comprehensive Hospital Information System developed using Oracle APEX and Oracle SQL Developer Data Modeler. This project includes database design, automated schema creation, a user-friendly interface, and role-based access control, aimed at optimizing hospital operations and improving data accuracy and efficiency.

## Project Overview

The Hospital Information System manages various hospital operations, including patient management, doctor assignments, treatment plans, and drug inventory management. The system is designed to optimize hospital workflows, improve data accuracy, and enhance overall efficiency.

## Features

- **Database Design and Management**: Utilizes Oracle SQL Developer Data Modeler to create a robust database schema.
- **Automated Schema Creation**: Generates SQL (DDL) from the data model and imports it into Oracle APEX.
- **User Interface Development**: Implements interactive UI pages for managing hospital data.
- **Role-Based Access Control**: Manages user roles and permissions within Oracle APEX.
- **Automated Inventory Management**: Includes triggers to manage drug inventory levels and automate order placements.

## Technologies Used

- **Oracle APEX**: Platform for developing enterprise applications with low-code capabilities.
- **Oracle SQL Developer Data Modeler**: Tool for visual database design and management.
- **SQL**: Used for database schema creation and data manipulation.
- **PL/SQL**: Used for creating triggers and managing sequences.

## Database Schema

The database schema includes the following tables:

- **Wings**: Stores information about hospital departments.
- **Wards**: Stores details about wards within each department.
- **Nurses**: Stores information about nurses, their assignments, and supervisors.
- **Doctors**: Stores details about doctors, their specialties, and team assignments.
- **Patients**: Stores patient information and emergency contact details.
- **Treatments**: Stores treatment details for patients.
- **Prescriptions**: Stores prescription details related to treatments and drugs.
- **Drugs**: Stores information about drugs and inventory levels.
- **MedicalProviders**: Stores information about drug suppliers.
- **OrderDrugs**: Stores details about drug orders.
- **DoctorSpecialities**: Stores information about various medical specialties.
- **Teams**: Stores information about medical teams and their contact details.

  ![Wings Managemen](images/database.jpg)

## Triggers

The system includes several triggers to automate certain operations and maintain data integrity:

- **trg_check_and_order_drugs**:
  - **Function**: Automatically places orders when drug stock levels fall below a specified threshold.
  - **Trigger Event**: After insert or update on the `prescriptions` table.

- **trg_prevent_exceed_nurses**:
  - **Function**: Ensures that the maximum number of nurses per ward is not exceeded.
  - **Trigger Event**: Before insert or update on the `nurses` table.

## UI Pages

The UI pages in Oracle APEX include:

1. **Login**:
   - **Description**: User authentication page.
   -   ![Login](images/Login.png)

2. **Wings Management**:
   - **Description**: Allows users to view, create, and edit hospital departments.
   -   ![Wings Managemen](images/Wings.png)
   -   ![Wings Managemen](images/ValidationWing.png)
   -   ![Wings Managemen](images/EditWing.png)

3. **Wards Management**:
   - **Description**: Allows users to view, create, and edit ward details.
   -   ![Wings Managemen](images/Wards.png)
   -   ![Wings Managemen](images/CreateWard.png)
   -   ![Wings Managemen](images/EditWard.png)
   - 
4. **Nurses Management**:
   - **Description**: Allows users to manage nurse assignments and roles.
   -   ![Wings Managemen](images/Nurses.png)
   -   ![Wings Managemen](images/CreateNurse.png)
   -   ![Wings Managemen](images/EditNurse.png)
     
5. **Patients Management**:
   - **Description**: Allows users to manage patient details and doctor assignments.
   -   ![Wings Managemen](images/Patients.png)
   -   ![Wings Managemen](images/CreatePatient.png)
   -   ![Wings Managemen](images/EditPatient.png)
     
6. **Teams Management**:
   - **Description**: Allows users to manage medical teams and contact information.
   -   ![Wings Managemen](images/Teams.png)
   -   ![Wings Managemen](images/CreateTeam.png)
   -   ![Wings Managemen](images/EditTeam.png)
     
7. **Treatments Management**:
   - **Description**: Allows users to manage treatment details for patients.
   -   ![Wings Managemen](images/Treatments.png)
   -   ![Wings Managemen](images/CreateTreatment.png)
   -   ![Wings Managemen](images/EditTreatment.png)
     
8. **MedicalProviders Management**:
   - **Description**: Allows users to manage drug suppliers.
   -   ![Wings Managemen](images/MedicalProviders.png)
   -   ![Wings Managemen](images/CreateMedicalProvider.png)
   -   ![Wings Managemen](images/EditMedicalProvider.png)
     
9. **OrderDrugs Management**:
   - **Description**: Allows users to manage drug orders and inventory.
   -   ![Wings Managemen](images/OrderDrugs.png)
   -   ![Wings Managemen](images/CreateOrderDrug.png)
   -   ![Wings Managemen](images/EditOrderDrug.png)
     
10. **Drugs Management**:
    - **Description**: Allows users to manage drug details and stock levels.
   -   ![Wings Managemen](images/Drugs.png)
   -   ![Wings Managemen](images/CreateDrug.png)
   -   ![Wings Managemen](images/EditDrug.png)
     
11. **DoctorSpecialities Management**:
    - **Description**: Allows users to manage doctor specialties.
   -   ![Wings Managemen](images/DoctorSpecialities.png)
   -   ![Wings Managemen](images/CreateDoctorSpecialitiy.png)
   -   ![Wings Managemen](images/EditDoctorSpecialitiy.png)
     
12. **Prescriptions Management**:
    - **Description**: Allows users to manage patient prescriptions.
   -   ![Wings Managemen](images/Prescriptions.png)
   -   ![Wings Managemen](images/CreatePrescription.png)
   -   ![Wings Managemen](images/EditPrescription.png)
  
  13. **Administration Management**:
    - **Description**: Administration Management.
   -   ![Wings Managemen](images/Administration.png)
     
## Installation and Setup

The project includes several SQL scripts to automate the database setup process. Follow the steps below to set up the database and deploy the application:

1. **Drop All Tables**:
   - Use the script `Drop all tables.sql` to drop all existing tables in the database.
   
2. **Drop All Sequences**:
   - Use the script `Drop all sequences.sql` to drop all existing sequences.

3. **Create Database Schema**:
   - Run the script `Create Database Schema.sql` to create the database schema.

4. **Create Sequences**:
   - Run the script `Create SEQUENCES.sql` to create the necessary sequences.

5. **Load Sample Data**:
   - Use the script `Sample Data.sql` to load sample data into the database.

6. **Deploy APEX Application**:
   - Import the application into Oracle APEX and configure the user roles and permissions.

## Contact

For any inquiries or access requests, please reach out via [LinkedIn](https://www.linkedin.com/in/pbernalis/) or email at [pbernalis@gmail.com](mailto:pbernalis@gmail.com).

## License
This project is licensed under the terms specified in this document. For more information, see the [LICENSE](https://github.com/pbernalis/pbernalis/blob/main/blob/main/License.md) file.
