# Performance Testing In JMeter
## Project Overview
This project performs load and stress tests using JMeter by simulating user actions like login, booking creation, and booking search to evaluate system performance. The generated HTML and Excel reports help analyze the results of the load and stress tests, highlighting throughput and identifying bottlenecks.

## ▶ Project Guidelines
Create a JMeter collection containing HTTP requests for the Login API, Create Booking API, and Search API. Include the following header property in the Header Controller:

○ Accept: `*/*`

### Login

○ URL : https://restful-booker.herokuapp.com/auth

○ Body:

  - "username": "admin",
  - "password": "password123"



### Create Booking

URL: `https://restful-booker.herokuapp.com/booking`

Body:

 - "firstname": "Generate Random FirstName",
 - "lastname": "Generate Random LastName",
 - "totalprice": "Generate random amount",
 - "depositpaid": true,
 - "bookingdates": {
  -  "checkin": "2024-01-01",
  -  "checkout": "2024-01-02"

 
 ### Search Booking
    ○ URL https://restful-booker.herokuapp.com/booking/<booking_id>

## 🚦 Project Scenario

This project performs performance testing on the Restful Booker API using Apache JMeter by simulating common user actions such as:

- 🔐 Logging into the system  
- 📝 Creating bookings with randomly generated data  
- 🔍 Searching for bookings using the booking ID  

The testing is divided into two key phases:

- ⚡ **Load Testing:** Simulates up to 120,000 users over a 12-hour period, compressed into 5, 10, and 20-minute intervals to assess system performance under expected load.  
- 💥 **Stress Testing:** Gradually increases the user load to determine the system’s breaking point and identify any bottlenecks.


## ▶ Tools and features
### 🛠️ Tools & Technologies Used  
🔧 Apache JMeter  
📊 Excel  
🎲 Random Variable Controller  
⏱️ Gaussian Timer  
📈 HTML Report Generation


## Screenshot of Load Test Report:
![loadreport](https://github.com/user-attachments/assets/7f8a12f8-5db8-41d2-920f-c213252d4e16)

## Screenshot of Stress Test Report :
![stressreport](https://github.com/user-attachments/assets/55069abe-1280-4ace-9b18-86893a509038)

## Excel Report of Load Test and Stress Test
[Click here for excel file](https://github.com/digonta-roy/Load-Test-and-Stress-Test-in-JMeter/blob/main/bookingLoad_Stress_Report.csv)

###### Caution : Remove Reports,Report(stress) folder and .jtl file when you run.
