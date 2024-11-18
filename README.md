# weverse
위버스 컴퍼니 팬참여 플랫폼 과제

# 📌 Project Name
팬참여 플랫폼 

---

## 🌟 Features

- 🔒 **Secure and Reliable**: Features for ensuring data integrity and security.
- 🚀 **High Performance**: Optimized to handle high volume of transactions smoothly.
- 📱 **Responsive Design**: Fully functional across devices and screen sizes.
- ⚙️ **Configurable**: Customizable settings for various user preferences.

---

## 🛠️ Technologies Used
- **Backend**: Java, Spring Boot, JPA, Kafka
- **Database**: H2 Database, Redis
---


## 📂 Project Structure

- **src/main/java/com/weverse/reservation/**: Main source code
  - **common/**: Common utility classes and configurations
    - **RedisConfig**: Redis configuration for distributed caching and locking
    - **ResponseData**: Standard API response wrapper
  - **controller/**: REST API controllers for handling requests
    - **BoothController**: Handles booth-related requests
    - **ConcertController**: Handles concert-related requests
    - **ReservationController**: Handles reservation-related requests
    - **UserController**: Handles user-related requests
  - **dto/**: Data Transfer Objects for request and response payloads
    - **BoothRequest**: DTO for booth-related requests
    - **ConcertRequest**: DTO for concert-related requests
    - **ReservationRequest**: DTO for reservation-related requests
    - **UserRequest**: DTO for user-related requests
  - **entity/**: JPA entities representing database tables
    - **BaseEntity**: Common fields for all entities (e.g., creation date)
    - **Booth**: Booth entity
    - **Concert**: Concert entity
    - **Reservation**: Reservation entity
    - **User**: User entity
  - **handler/**: Custom exception handlers
    - **ApiExceptionHandler**: Handles application-wide exceptions
  - **repository/**: JPA repositories for data access
    - **BoothRepository**: Repository for `Booth` entity
    - **ConcertRepository**: Repository for `Concert` entity
    - **ReservationRepository**: Repository for `Reservation` entity
    - **UserRepository**: Repository for `User` entity
  - **service/**: Service layer for business logic
    - **BoothService**: Service for booth operations
    - **ConcertService**: Service for concert operations
    - **ReservationService**: Service for reservation operations
    - **UserService**: Service for user operations
    - **kafka/**: Kafka-related services
      - **ConsumerService**: Kafka consumer for reservation requests
      - **ProducerService**: Kafka producer for event publishing
- **resources/db/**: Database initialization scripts
  - **data.sql**: Initial data for database setup
  - **test-data.sql**: Test data for development/testing purposes
- **resources/static/**: Static web assets (e.g., HTML, CSS, JS)
- **resources/templates/**: HTML templates for server-side rendering
- **application.properties**: Application configuration properties


---




