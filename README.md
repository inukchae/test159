# weverse
위버스 컴퍼니 팬참여 플랫폼 과제

# 📌 Project Name
팬참여 플랫폼 

---

## 🌟 Features

 동시에  10,000명의 요청에 대해서 선착순 100명의 요청만 예약 하는 서비스 로직


---

## 🛠️ Technologies Used
- **Backend**: Java, Spring Boot, JPA, Kafka
- **Database**: H2 Database, Redis
---


## 📂 Project Structure

<img width="408" alt="image" src="https://github.com/user-attachments/assets/5a58d311-9dde-4640-b1e0-6a8705cfbbdf">


---

## 📊 UML Diagram
<img width="836" alt="image" src="https://github.com/user-attachments/assets/a4d8edd5-cd08-468c-a137-58abec239269">

```plantuml
@startuml
actor User
participant "ReservationController" as RC
participant "ReservationService" as RS

User -> RC: Send reservation request
RC -> RS: Process reservation request
RS -> RC: Return reservation result
RC -> User: Send reservation response
@enduml
```

This PlantUML diagram shows the interaction between a user and the reservation system. The user sends a request to the `ReservationController`, which then communicates with the `ReservationService` to process the reservation and return the result.











