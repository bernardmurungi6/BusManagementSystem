# Bus Management System — OOP Java Assignment

## Project Structure
```
BusManagementSystem/
├── Dockerfile
├── pom.xml
└── src/main/java/com/busms/
    ├── interfaces/
    │   ├── Bookable.java
    │   └── Trackable.java
    ├── model/
    │   ├── Vehicle.java          ← Abstract class
    │   ├── BusManager.java       ← Extends Vehicle, implements Bookable & Trackable
    │   ├── CityBus.java
    │   ├── ExpressBus.java
    │   ├── LuxuryBus.java
    │   ├── SchoolBus.java
    │   ├── TouristBus.java
    │   ├── ElectricBus.java
    │   ├── Passenger.java
    │   ├── Driver.java
    │   ├── Route.java
    │   ├── Ticket.java
    │   ├── Booking.java
    │   ├── Payment.java
    │   ├── Schedule.java
    │   └── Maintenance.java
    ├── factory/
    │   └── BusFactory.java
    ├── report/
    │   └── ReportGenerator.java
    ├── util/
    │   └── InputValidator.java
    └── main/
        └── BusSystem.java        ← Main entry point
```

## OOP Concepts Demonstrated
| Concept        | Where                                      |
|----------------|--------------------------------------------|
| Encapsulation  | All model classes (private fields + getters/setters) |
| Abstraction    | `Vehicle.java` (abstract class)            |
| Interfaces     | `Bookable.java`, `Trackable.java`          |
| Inheritance    | BusManager → 6 subclasses                 |
| Polymorphism   | `BusFactory`, overridden methods           |
| Constructors   | Default + parameterized in every class     |
| Method Override| `toString()`, `calculateFare()`, `startVehicle()`, etc. |

