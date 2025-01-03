<h1>Bank Management System</h1>

Welcome to the Bank Management System project repository! This collaborative effort aims to provide a comprehensive solution for managing banking operations efficiently. We've successfully implemented both the front-end and back-end components, with a focus on user-friendly interfaces and robust backend functionality.

<h3>Technologies Used</h3>
Frontend: Angular, TypeScript, HTML, Tailwind CSS<br>
Backend: Spring Boot, Java, Spring Data JPA, Maven, JAVA JDK 17, REST API.<br>
Database: Oracle<br>

<h3>Getting Started</h3>
* Clone the repository.<br>
* Refresh maven file. <br>
* Set up the property: Edit and enter your database username password. <br>
* Run the application: The API should now be running at localhost.<br>
* Set up the frontend: Follow the instructions in the frontend/README.md file.<br>

<h3>Endpoints</h3>

Sign Up:

Endpoint: POST '/customer/signup'<br>
Description: Register a new customer.<br>
Request Body: Customer object.<br>

Login:

Endpoint: POST '/customer/login'<br>
Description: Authenticate a customer.<br>
Request Body: CustomerWrapper object containing username and password.<br>

Get All Customers:

Endpoint: GET '/customer/get'<br>
Description: Retrieve a list of all customers.<br>

Get Customer by Username:

Endpoint: GET '/customer/get/{username}'<br>
Description: Retrieve a customer by their username.<br>
Path Variable: username<br>

Check Username Availability:

Endpoint: GET '/customer/{username}'<br>
Description: Check if a username is available.<br>
Path Variable: username<br>

Get All Transactions:

Endpoint: GET '/customer/gettransactions'<br>
Description: Retrieve a list of all transactions.<br>

Get Transactions by Username:

Endpoint: GET '/customer/transactions/{username}'<br>
Description: Retrieve transactions for a specific customer.<br>
Path Variable: username<br>

Save Transaction:

Endpoint: POST '/customer/transactions/{username}'<br>
Description: Save a new transaction for a customer.<br>
Path Variable: username
Request Body: Transaction object.
Bill Payment:

Endpoint: PUT '/customer/billpayment/{username}'<br>
Description: Process a bill payment for a customer.<br>
Path Variable: username<br>
Request Parameters: amount, billerWrapper (as request body).<br>

Delete Customer:

Endpoint: DELETE '/customer/delete/{username}'<br>
Description: Delete a customer.<br>
Path Variable: username<br>

Deposit:

Endpoint: PUT '/customer/deposit'<br>
Description: Deposit funds into a customer's account.<br>
Request Parameters: username, amount<br>

Withdraw:

Endpoint: PUT '/customer/withdraw'<br>
Description: Withdraw funds from a customer's account.<br>
Request Parameters: username, amount<br>

Update Customer Password:

Endpoint: PUT '/customer/updateCustomerPassword'<br>
Description: Update a customer's password.<br>
Request Parameters: username<br>
Request Body: Map containing currentPassword and newPassword.<br>

Fund Transfer:

Endpoint: PUT '/customer/fundTransfer'<br>
Description: Transfer funds between customer accounts.<br>
Request Parameters: senderUsername, receiverAccountNo, amount<br>

<h1>Thank You</h1>
