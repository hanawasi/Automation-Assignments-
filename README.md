API Testing using Postman and JMeter

Project Overview

This project contains API testing using Postman and performance/load testing using Apache JMeter.

The APIs used in this project are based on JSONPlaceholder.

 Postman API Testing

The Postman collection contains the following API requests:

1. GET - All Users

    Retrieves the list of all users.
2. GET - User with Specific ID

    Retrieves a user using a specific user ID.
3. POST - New User

   Creates a new user.
4. PUT - Update ID 4 User

    Updates the user with ID 4.
5. DELETE - Delete ID 5 User

   Deletes the user with ID 5.
6. GET - New Request

    Additional GET request for API testing.

 How to Run Postman Tests

1. Open Postman.
2. Import the Postman Collection JSON file.
3. Open the collection.
4. Run the requests individually or use the Collection Runner.
5. Check the response status, response body, and test results.

 JMeter Performance Testing

The JMeter test plan is created to perform performance/load testing on the JSONPlaceholder API using virtual users.

JMeter Test Plan Structure

The test plan contains the following components:

 Virtual Users (Thread Group)
Used to configure the number of virtual users and control how the test is executed.

JSONPlaceholder (HTTP Request Sampler)
Used to send HTTP requests to the JSONPlaceholder API.

View Results Tree (Listener)
Used to view individual request results, response codes, and response data.

Summary Report (Listener)
Used to view the overall performance statistics of the test.

JMeter Components

| Component         | Type                 | Purpose                                             |
| ----------------- | -------------------- | --------------------------------------------------- |
| Virtual Users     | Thread Group         | Simulates virtual users and controls test execution |
| JSONPlaceholder   | HTTP Request Sampler | Sends HTTP requests to the API                      |
| View Results Tree | Listener             | Displays individual request and response details    |
| Summary Report    | Listener             | Displays overall performance statistics             |

How to Run JMeter Tests

1. Open Apache JMeter.
2. Open the `.jmx` test plan included in the repository.
3. Check the Virtual Users (Thread Group) settings.
4. Click Run.
5. Open View Results Tree to inspect individual request responses.
6. Open Summary Report to view overall performance statistics such as:

   * Number of Samples
   * Average Response Time
   * Minimum Response Time
   * Maximum Response Time
   * Error Percentage
   * Throughput

JMeter Test Results

Screenshots/reports of the JMeter test execution are included.

The results demonstrate the API performance during the execution of the configured virtual users.
