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
 
## Screenshot of Load Test Report:
