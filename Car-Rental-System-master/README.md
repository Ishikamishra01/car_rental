# Car Rental System

## Overview

The Car Rental System is a simple console-based application for managing car rentals. It allows customers to rent and return cars while tracking available cars and ongoing rentals.

## Features

- **Rent a Car**: View available cars and rent one for a specified number of days.
- **Return a Car**: Return a rented car and update its availability status.
- **Customer Management**: Automatically generate a unique customer ID and keep track of customer names.
- **Price Calculation**: Calculate the rental cost based on the number of days and the car's base price per day.

## Classes

### `Car`

Represents a car in the rental system.

- **Attributes**:
  - `carId`: Unique identifier for the car.
  - `brand`: Brand of the car.
  - `model`: Model of the car.
  - `basePricePerDay`: Base rental price per day.
  - `isAvailable`: Availability status of the car.
  
- **Methods**:
  - `calculatePrice(int rentalDays)`: Calculates the rental price based on the number of days.
  - `rent()`: Marks the car as rented.
  - `returnCar()`: Marks the car as available.

### `Customer`

Represents a customer in the rental system.

- **Attributes**:
  - `customerId`: Unique identifier for the customer.
  - `name`: Name of the customer.
  
- **Methods**:
  - `getCustomerId()`: Returns the customer ID.
  - `getName()`: Returns the customer's name.

### `Rental`

Represents a rental transaction.

- **Attributes**:
  - `car`: The car being rented.
  - `customer`: The customer renting the car.
  - `days`: Number of days for which the car is rented.

- **Methods**:
  - `getCar()`: Returns the rented car.
  - `getCustomer()`: Returns the customer who rented the car.
  - `getDays()`: Returns the number of rental days.

### `CarRentalSystem`

Manages the overall car rental process including adding cars, renting and returning cars, and handling user interactions.

- **Attributes**:
  - `cars`: List of available cars.
  - `customers`: List of customers.
  - `rentals`: List of ongoing rentals.

- **Methods**:
  - `addCar(Car car)`: Adds a car to the system.
  - `addCustomer(Customer customer)`: Adds a customer to the system.
  - `rentCar(Car car, Customer customer, int days)`: Rents a car to a customer.
  - `returnCar(Car car)`: Returns a car to the system.
  - `menu()`: Displays the user interface for interacting with the system.

## Usage

1. **Run the Program**: Execute the `Main` class to start the Car Rental System.
2. **Choose an Option**: Use the console menu to rent a car, return a car, or exit the program.
3. **Follow Prompts**: Enter required information such as car ID, customer name, and rental days as prompted.

## Example

