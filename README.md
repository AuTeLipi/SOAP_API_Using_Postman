# SOAP_API_Using_Postman
🧼 Manual SOAP API Testing for ISBN-10 Verification | Postman Edition

This repository contains a comprehensive manual testing suite for the SOAP-based ISBN validation API (IsValidISBN10) provided by DataFlex Web Services. The objective is to test the correctness, robustness, and behavior of the service using raw XML SOAP requests in Postman.

📌 Key Features:

🧪 30+ manually executed test cases using Postman:
   - Valid ISBN-10 (with and without hyphens).
   - ISBNs ending with 'X' as checksum.
   - Invalid inputs (short/long, special characters, alphabetic, alphanumeric).
   - Negative scenarios: empty, null, missing headers, malformed body.
        
  📬 Built entirely with Postman using the Desktop Agent.
  ✅ Validates response payloads and HTTP status codes (200, 400, 415, 500).
  🧾 Custom SOAPAction headers and raw XML request bodies configured manually.

📂 Repository Structure:
   - /TestCases/ → XLSX file with detailed test cases (TC001–TC034)
   - /Postman_Setup/ → Sample screenshots and header configuration
   - /SOAP_Requests/ → Raw XML payloads for various ISBN scenarios
   - /Docs/ → Test Plan, WSDL reference, and result analysis

🛠 Tools & Technologies:
    - Postman (Desktop App)
    - SOAP protocol (1.1)
    - XML + WSDL analysis
    - Manual test execution & logging in Excel

🧑‍💻 How to Run:
   1. Clone this repository locally.
   2. Open Postman and switch to the Desktop Agent.
   3. Set request type to POST and enter this endpoint:
      - https://webservices.daehosting.com/services/isbnservice.wso
   4. Under Headers, set:
        - Content-Type: text/xml; charset=utf-8
   5. Under Body tab:
        - Choose raw and select XML as type.
        - Paste the SOAP envelope from the /SOAP_Requests folder.
   6. Click Send and verify the boolean response & HTTP status.
   7. Log your result in the /TestCases sheet.

📌 Ideal For:
   - QA/Test Engineers practicing manual API validation.
   - Demonstrating SOAP testing skills using modern tools like Postman.
   - Creating baseline functional coverage for legacy web services.
