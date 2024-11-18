

위버스 컴퍼니 팬참여 플랫폼 과제

# 📌 Project Name
팬참여 플랫폼 


## 🌟 Features
 동시에  10,000명의 요청에 대해서 선착순 100명의 요청만 예약 하는 서비스 로직

 
---


## 🛠️ Technologies Used
- **Backend**: Java, Spring Boot, JPA, Kafka
- **Database**: H2 Database, Redis

1.데이터베이스 접근을 기다리지 않게 하고, 데이터베이스의 락으로 인해 발생할 수 있는 요청 대기 문제를 방지하기 위해, 메시지 큐(카프카)를 이용한 비동기 처리
2.여러 스레드, 혹은 여러 인스턴스로 부터의 선착순 100명을 카운팅하기 위한 동시성 처리를 위해  Redis의 INCR 명령을 통한 원자적 처리
---


## 📂 Project Structure

<img width="408" alt="image" src="https://github.com/user-attachments/assets/5a58d311-9dde-4640-b1e0-6a8705cfbbdf">

---

## 📊 UML Diagram
<img width="836" alt="image" src="https://github.com/user-attachments/assets/a4d8edd5-cd08-468c-a137-58abec239269">



---

## 📈 Test Cases

<img width="1619" alt="image" src="https://github.com/user-attachments/assets/d20e6d7e-1ce5-4ca0-805b-ea6a883cc641">
<img width="996" alt="image" src="https://github.com/user-attachments/assets/db39e2f1-3322-421e-ae53-c4b8c42cb86c">









