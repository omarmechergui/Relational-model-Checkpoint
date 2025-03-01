# Relational-model-Checkpoint
# Hotel Management Database

## Overview
This project involves designing and implementing a relational database for managing hotel information. The database is created by converting an Entity-Relationship (ER) model into a relational schema.

## Objectives
- Transform the provided ER diagram into a relational database schema.
- Establish tables, attributes, primary keys, and relationships.
- Ensure the database supports hotel operations such as managing rooms, customers, and reservations.

## Database Structure
The database consists of the following tables:

1. **Hotel**
   - hotel_id (Primary Key)
   - name
   - address
   - rating

2. **Room**
   - room_id (Primary Key)
   - hotel_id (Foreign Key references Hotel)
   - room_number
   - room_type
   - price

3. **Customer**
   - customer_id (Primary Key)
   - first_name
   - last_name
   - phone_number
   - email

4. **Reservation**
   - reservation_id (Primary Key)
   - customer_id (Foreign Key references Customer)
   - room_id (Foreign Key references Room)
   - check_in_date
   - check_out_date

## Requirements
- Database Management System (e.g., MySQL, PostgreSQL, SQLite)
- SQL knowledge for creating tables and establishing relationships

## Installation
1. Clone the repository:

    ```bash
    git clone <repository-url>
    cd hotel-management-db
    ```

2. Set up the database schema using the provided SQL script:

    ```bash
    psql -U username -d hotel_db -f schema.sql
    ```

## Usage
- Perform CRUD operations on hotels, rooms, customers, and reservations.
- Query the database for reservation details and availability.

## Contributing
Contributions are welcome! Feel free to submit a pull request with enhancements or bug fixes.

## License
This project is licensed under the MIT License.

## Contact
For questions or support, reach out to (mailto:oo2377107@gmail.com).

