# Car Rental System

This Java-based Car Rental System allows users to rent and return cars. It manages the cars, customers, and rentals, providing a user-friendly interface via the command line. The system enables customers to view available cars, rent them for a specified number of days, and return them once they are done.

## Features

- **Rent a Car**: Customers can select an available car and rent it for a specified number of days. The system calculates the total rental price based on the car’s daily rate.
- **Return a Car**: Customers can return rented cars, marking them as available for other users.
- **Menu-based Interface**: A simple text-based menu is presented to the user for navigation.
- **Car Management**: The system supports adding cars, each with unique details like brand, model, and base price per day.
- **Customer Management**: Customers are assigned unique IDs upon renting a car, and their information is stored in the system.

## Requirements

- Java 8 or later
- Command-line interface for running the program

## File Structure

- `Car.java`: Contains the details and methods related to cars in the system (ID, brand, model, base price per day, availability, etc.).
- `Customer.java`: Contains the details of customers such as ID and name.
- `Rental.java`: Represents a rental transaction, linking cars and customers for a specific number of rental days.
- `CarRentalSystem.java`: The core system logic, responsible for managing cars, customers, and rentals.
- `Car_Rental_System.java`: The main class with the entry point for running the program.

## How to Use

1. Clone the repository or download the project files.
2. Open the terminal/command prompt.
3. Navigate to the folder containing the `.java` files.
4. Compile the Java files:
    ```bash
    javac Car.java Customer.java Rental.java CarRentalSystem.java Car_Rental_System.java
    ```
5. Run the program:
    ```bash
    java Car_Rental_System
    ```

6. Interact with the system by following the on-screen prompts:
    - **1. Rent a Car**: Rent an available car by entering the car ID and rental days.
    - **2. Return a Car**: Return a rented car by entering the car ID.
    - **3. Exit**: Exit the system.

### Example Interaction:
```plaintext
===== Car Rental System =====
1. Rent a Car
2. Return a Car
3. Exit
Enter your choice: 1

== Rent a Car ==

Enter your name: John Doe

Available Cars:
ID_001 - BMW BMW X3
ID_002 - AUDI AUDI Q3
ID_003 - Mahindra Thar
ID_004 - Suzuki Brezza
ID_005 - Hyundai I 10

Enter the car ID you want to rent: ID_003
Enter the number of days for rental: 5

== Rental Information ==

Customer ID: CUS1
Customer Name: John Doe
Car: Mahindra Thar
Rental Days: 5
Total Price: $6000.00

Confirm rental (Y/N): Y

Car rented successfully
