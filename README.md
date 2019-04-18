#Sample Phone Directory Service APIs:
------------------------------------

Language : Java 8
Technology: Spring Boot
Author: Kannan Gnanasigamani


APIs:

1) API to get all the availabe PhoneNumbers - GET request
---------------------------------------------------------
http://localhost:8085/phoneDirectory/api/availablePhoneNumbers

2) API to get all the PhoneNumbers for a customer - GET request
---------------------------------------------------------------
http://localhost:8085/phoneDirectory/api/{customerId}/phoneNumbers

3) API to activate a PhoneNumber for a customer - POST request
--------------------------------------------------------------
http://localhost:8085/phoneDirectory/api/activate


Steps:
1) Get all the available phone numbers using the first API      
Example: http://localhost:8085/phoneDirectory/api/availablePhoneNumbers

2) Get all the phone numbers for A customer using the second API
Example: http://localhost:8085/phoneDirectory/api/111/phoneNumbers

3) Activate a phone number for a customer using the third API
Example:  http://localhost:8085/phoneDirectory/api/activate

with body: 
{
"customerId" : 111,
"phoneNumber": "0723456789"
}


NOTE: Use POSTMAN for the results.
