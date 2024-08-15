# Broward County Transit Bus App

This is my Java Spring application that tells users when the next Broward County (Florida) transit bus is arriving at a specific stop.

## Features

- **Real-time Bus Arrival Information**: The app fetches and displays the next bus times for a given stop.
- **RESTful API**: I've implemented a simple REST API to interact with the app.
- **Easy to Extend**: I've designed the app so that it can be easily extended with additional features like user authentication, more detailed transit data, and a frontend interface.

## Getting Started

### Prerequisites, Installation, and Usage

Before you can run the app, you'll need the following:

1. **Prerequisites**:
    - **Java Development Kit (JDK) 8+**
    - **Maven** or **Gradle** for dependency management
    - An IDE like **IntelliJ IDEA** or **Eclipse**
    - A Broward County Transit API key (or a key from a third-party service providing bus data)

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/broward-transit-app.git
   cd broward-transit-app
   ```

3. **Configure Application Properties**:
    - Open `src/main/resources/application.properties` and add your API key:
      ```properties
      transit.api.key=YOUR_API_KEY_HERE
      transit.api.url=https://api.broward.org/transit
      ```

4. **Build the Project and Run the Application**:
    - If you're using Maven:
      ```bash
      mvn clean install
      mvn spring-boot:run
      ```
    - If you're using Gradle:
      ```bash
      gradle build
      ```

Once the application is running, you can access the API endpoint to get the next bus times. For example:

```
GET http://localhost:8080/next-bus?stopId=1234
```

This will return the next bus arrival times for the stop with ID `1234`.

## Future Enhancements

I plan to add the following features:

- **User Authentication**: Secure the API so that only authorized users can access it.
- **Frontend Interface**: Build a user-friendly web interface to interact with the API.
- **Detailed Transit Data**: Include additional information like route details and service alerts.

## Contributing and Contact

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. If you have any questions or suggestions, feel free to contact me at [evon.codes@gmail.com](mailto:evon.codes@gmail.com).

