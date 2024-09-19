# flight-booking-system

## Project Description
The **flight-booking-system** is a comprehensive C++ application designed to simulate a flight booking and management system. It utilizes advanced data structures like hash tables and linked lists to efficiently store and manage flight and ticket information. This project is a demonstration of my skills in C++ programming, data structure implementation, and modular code organization.

## Implementation Details

### Key Features

1. **Hash Table for Flight Management:**
   - The system uses a custom hash table implementation (`flighthashtable`) to store and manage flight information. This ensures constant time complexity for flight lookup, insertion, and deletion operations.
   - Each flight entry in the hash table includes details such as flight number, destination, and availability.

2. **Linked List for Ticket Management:**
   - A custom linked list implementation (`mylist`) is used to manage the flight tickets. This structure allows dynamic memory allocation and efficient ticket management.
   - Tickets can be created, viewed, and deleted. Each ticket is linked to a specific flight stored in the hash table.

3. **Modular Design:**
   - The project is divided into multiple modules, each encapsulated in separate `.cpp` and `.h` files. This makes the code more maintainable and easier to extend.
   - The `main` module integrates all functionalities and provides a user interface to interact with the system.

4. **Efficient Memory Management:**
   - Proper use of pointers and dynamic memory allocation ensures efficient memory usage and prevents memory leaks.
   - The destructor methods in each class ensure that all dynamically allocated memory is properly freed.

5. **User-Friendly Interface:**
   - The system provides a simple text-based user interface for interacting with the flight and ticket management functionalities.
   - Users can perform various operations such as adding new flights, booking tickets, and viewing flight details.

### Implementation Modules

- **`flighthashtable.h` & `flighthashtable.cpp`:** Implements a custom hash table for storing flight details. The hash function is designed to distribute flights evenly across the table, minimizing collisions and ensuring efficient data retrieval.

- **`flightticket.h` & `flightticket.cpp`:** Manages flight tickets. The `FlightTicket` class includes methods for creating and managing tickets, each linked to a specific flight.

- **`mylist.h`:** Implements a custom linked list to store ticket information. This data structure supports dynamic allocation and is used extensively in the ticket management module.

- **`main.cpp`:** The main entry point of the program, integrating all modules and providing the user interface for interaction.

## How to Build and Run

### Prerequisites
- `g++` compiler
- `make` utility

### Build Instructions

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/FlightBookingSystem.git
    cd FlightBookingSystem
    ```

2. Build the project using `make`:
    ```bash
    make
    ```

3. Run the application:
    ```bash
    ./output
    ```

### Directory Structure

- **`include/`**: Contains header files for all modules.
- **`src/`**: Contains source files for all modules.
- **`obj/`**: (Optional) Contains object files generated during compilation.
- **`Makefile`**: Automates the build process.
- **`README.md`**: Documentation of the project.

## Potential Improvements

- **Persistent Storage:** Implement database integration to store flight and ticket information persistently.
- **User Authentication:** Add user authentication to distinguish between admin and customer roles.
- **GUI Development:** Create a graphical user interface to improve user interaction and experience.

## Learning Outcomes
This project enhanced my understanding of data structures, especially hash tables and linked lists. It also helped me practice modular programming and efficient memory management in C++. I gained experience in organizing code for scalability and maintainability.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
