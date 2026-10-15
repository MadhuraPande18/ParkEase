## ☕ Core Java & OOP concepts

| Concept | How ParkEase uses it |
|---------|----------------------|
| **Abstraction** | Abstract `Vehicle` and `ParkingSpot` classes define what every vehicle and spot must provide |
| **Inheritance** | `Bike`, `Car`, `Truck` extend `Vehicle`; `BikeSpot`, `CarSpot`, `TruckSpot` extend `ParkingSpot` |
| **Polymorphism** | Method overriding (`display()`, `canFitVehicle()`) and runtime polymorphism through strategy interfaces |
| **Encapsulation** | Private state, exposed only through controlled methods such as `parkVehicle()` and `removeVehicle()` |
| **Interfaces** | `ParkingStrategy`, `PricingStrategy`, `PaymentStrategy`, `ParkingObserver` |
| **Composition** | A `ParkingLot` has floors, a floor has spots, a ticket has a vehicle and a spot |
| **Enums** | `VehicleType`, `SpotType`, `TicketStatus` for type-safe constants |
| **Collections Framework** | `HashMap` for O(1) lookup by ticket and by vehicle number, `ArrayList` for floors and spots |
| **Exception handling** | Business rules such as *Parking is full* and *already parked* raised as exceptions and returned as clear API errors |
| **Java Time API** | `LocalDateTime` and `Duration` for entry/exit times and hourly billing |
| **Static & synchronized** | Static ticket counter and a `synchronized` Singleton `getInstance()` |
| **Lambdas & functional interfaces** | REST routes registered as lambdas in the API server |

---
