# Employee Address Application

## Frameworks and Language Used
- Framework: Spring Boot
- Language: Java
- Database: [MySQL]

## Data Flow

### Controller
- `GET /employees` - Get all employees
- `GET /employees/{id}` - Get an employee by ID
- `POST /employees` - Create a new employee
- `PUT /employees/{id}` - Update an employee by ID
- `DELETE /employees/{id}` - Delete an employee by ID

- `GET /addresses` - Get all addresses
- `GET /addresses/{id}` - Get an address by ID
- `POST /addresses` - Create a new address
- `PUT /addresses/{id}` - Update an address by ID
- `DELETE /addresses/{id}` - Delete an address by ID

### Services
- `EmployeeService`: Contains methods for handling employee-related business logic.
- `AddressService`: Contains methods for handling address-related business logic.
### Repository
- `EmployeeRepository`: Provides data access methods for the Employee entity.
- `AddressRepository`: Provides data access methods for the Address entity.
### Database Design
- Employee Table:
  - `id` (Primary Key, Long)
  - `firstName` (String)
  - `lastName` (String)
  - `address_id` (Foreign Key, Long, referencing Address Table)
- Address Table:
  - `id` (Primary Key, Long)
  - `street` (String)
  - `city` (String)
  - `state` (String)
  - `zipcode` (String)
### Data Structure Used
- Employee (Entity class): Represents an employee with attributes such as id, firstName, lastName, and an associated Address.


- Address (Entity class): Represents an address with attributes such as id, street, city, state, and zipcode.





## Project Summary
- This Employee Address application is built using Spring Boot and Java.
- It allows users to perform CRUD operations on User, Product, Address, and Order entities.
- The project follows a structured architecture with controllers, services, and repositories.
- Data is stored in a MySQL database with appropriate relationships.
- The API is designed to handle user registration, product management, order placement, and more.