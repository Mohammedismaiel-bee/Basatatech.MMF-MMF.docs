Project Phases and Tasks:

#### 1. Database Design:

- Design the Money Market Fund (MMF) Transaction Database to log all transactions (inbound and outbound) and their details.
- Define transaction types and statuses.
- Create the MMF Customer Database, defining customer types and statuses.

#### 2. Management Interface Development:

- Develop a management interface on the CCOffice platform for handling MMF customers.
  This includes the development of a web UI for customer management and monitoring.
- Create a web UI for managing (maker/checker), monitoring MMF transactions, and generating reports.

#### 3. Connect Phase:

- design connect architecture

- analize the new database architecture

- extract the connect input parameters

- extract the connect output parameters

- configure the database connection to write and listen for notifications

- configure the connect (add configuration in the CC database for the connect)

- explore the MMF documents to fully understand the requirements

- explore the CIC swagger documents for extracting [CIC APIs](https://mobdev.teacomputers.com/fitsapi/swagger/index.html?urls.primaryName=Fund)

#### 4. Customer Mobile Server:

- Integrate the MMF system with a Know Your Customer (KYC) system to verify customer identities.
- Adopt the "Pay2Collect" payment method for customer transactions.
- Implement bank card integration for seamless payment processing.
- Develop the backend for the user interface (UI) on the customer mobile server,incorporating core functionalities of the MMF system:
  - Adding new customers to the system.
  - Checking customer account balances.
  - Adding funds to customer accounts.
  - Processing withdrawals:
    - To Bank accounts:
      - Finalize the Automated Clearing House (ACH) integration with the Payment Gateway (PGW).
      - Develop an API on the PGW side to transfer funds.
      - Consume the API from the CCOffice side to disburse funds to customers for withdrawals to their bank accounts.
    - To Vodafone (VDF) Wallet:
      - Investigate the availability of an API for VDF Wallet integration, or consider using the same API used for bank transactions.

#### 5. APK (Mobile Application):

a. Implement the user interface (UI) for the entire frontend of the Money Market Fund (MMF) mobile application.
b. Integrate the KYC system into the mobile app to ensure customer identity verification.
