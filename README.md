Smart Wood Production Monitoring System
1. Project Overview
The Smart Wood Production Monitoring System is an Android application and web-based interface concept designed to support the daily operations of a wood production business. The project is developed for the Sonae Arauco project context and focuses on making production information, customer orders, product prices, quotation requests, machine maintenance, and reports easier to access and manage.
The system provides two main areas:
Customer area: Customers can browse products and prices, submit an order, track an order using their order reference and email address, and send a quotation request.
Employee/manager area: Authorised users in the demonstration interface can view customer orders and quotation requests, update order statuses, manage displayed prices, review sample production and machine information, view reports, and manage selected settings.
The purpose of the project is to demonstrate how a digital system can bring important production and customer-service tasks together in one place. It is intended as a prototype and learning project, and further development is needed before it can be used as a live production system.
2. Project Objectives
The main objectives of the Smart Wood Production Monitoring System are to:
Provide a simple interface for customers and employees.
Display wood products and their listed prices.
Allow customers to submit order details electronically.
Allow customers to look up order information using an order reference and email address.
Allow customers to submit quotation requests.
Provide an employee workspace for reviewing orders and quotation requests.
Demonstrate order-status updates and basic price management.
Display sample production and machine information.
Present maintenance scheduling and reporting features.
Provide settings for basic profile preferences, notifications, and theme selection.
Demonstrate how a mobile application can present business functions through a straightforward interface.
3. Main Features
3.1 Home Dashboard
The home screen introduces the system and provides navigation to the main customer and employee functions.
3.2 Products and Prices
Customers can view the products and prices displayed in the application. The values currently shown are demonstration data and should be checked and replaced with approved, current business information before any real-world use.
3.3 Customer Orders
Customers can complete an order form and submit the required details. The application can display an order reference so the customer can look up the order later on the same device where the data is stored.
3.4 Order Tracking and Details
The order-tracking area allows a customer to enter an order reference and email address to find the matching saved order details. Order tracking is based on locally stored demonstration data; it does not retrieve live information from a company server.
3.5 Quotation Requests
Customers can submit a request for a quotation by providing the requested contact and product information. In the current prototype, the request is stored locally rather than being automatically sent to Sonae Arauco or another company system.
3.6 Employee Sign-In and Workspace
The application includes a demonstration employee sign-in and a workspace for viewing saved orders and quotation requests. The sign-in is intended for demonstrating navigation and is not production-grade authentication. Do not use real or confidential passwords with this prototype.
3.7 Order Management
The employee workspace can show order information and demonstrate changing an order's status. Because the data is local to the device/browser storage, changes are not shared with other devices or users.
3.8 Price Management
The prototype demonstrates editing displayed product prices. The prices are sample values and should not be treated as official quotations or binding sales prices.
3.9 Production and Machine Information
The system includes sample production and machine information to illustrate how a manager might review operational data. These values are not connected to factory machines, sensors, or a live production database.
3.10 Maintenance Scheduling
The maintenance area demonstrates how maintenance tasks may be presented and scheduled. It is a prototype feature and does not currently send tasks to a maintenance-management service.
3.11 Reports and Export
The reports section presents example operational summaries and supports exporting available report data as a CSV file where the feature is provided. The exported information is based on data available within the local prototype and should not be treated as a verified business report.
3.12 Settings
The settings area provides basic preferences such as the displayed profile name, notification preference, and light/dark theme. These settings are intended for demonstration purposes.
3.13 Contact Information
The application includes the following Sonae Arauco South Africa commercial office details:
Commercial Office  
Building 18, 1st Floor, Woodlands Office Park  
20 Woodlands Drive, Woodmead, 2157  
South Africa
Telephone: (+27) 11 236 1400
Fax: (+27) 11 236 1440
Email: info.southafrica@sonaearauco.com
Please confirm the contact details with the organisation before using them for official communication.
4. Technology Stack
The project uses the following technologies:
Android Studio: The development environment used to open and work on the Android project.
Java: Used for the Android application shell and WebView activity.
HTML: Defines the structure of the application's screens.
CSS: Controls the layout, styling, and responsive presentation.
JavaScript: Handles interface interactions and prototype functions.
Android WebView: Displays the HTML, CSS, and JavaScript interface inside the Android application.
Local storage: Stores demonstration information on the device/browser environment.
The exact tools and versions may depend on the Android Studio and Gradle configuration used to open the project.
5. Project Structure
The Android project contains files and folders similar to the following:
```text
SmartWoodAndroid/
├── app/
│   ├── build.gradle
│   └── src/
│       └── main/
│           ├── AndroidManifest.xml
│           ├── java/
│           │   └── com/
│           │       └── smartwood/
│           │           └── app/
│           │               └── MainActivity.java
│           ├── res/
│           │   └── values/
│           │       └── styles.xml
│           └── assets/
│               └── www/
│                   ├── index.html
│                   ├── styles.css
│                   └── app.js
├── build.gradle
├── settings.gradle
├── gradle.properties
└── README.md
```
The exact file names may vary slightly depending on which project version is being used. The `MainActivity.java` file starts the Android interface, while the web files inside `assets/www/` provide the screens and client-side interactions.
6. How to Open the Project in Android Studio
Download the project ZIP file from the repository or the location where it was shared.
Extract the ZIP file to a folder on your computer.
Open Android Studio.
Select Open from the welcome screen, or use File → Open.
Choose the extracted project folder containing `settings.gradle`.
Allow Android Studio to synchronise the Gradle files.
If Android Studio asks to install a required Android SDK or build tool, review the prompt and install the required component.
Wait for synchronisation to finish and check the Build window for errors.
Connect an Android phone with USB debugging enabled, or create and start an Android emulator.
Select the device in Android Studio and press Run.
If the project does not build, review the error message and confirm that the Android Gradle Plugin, Gradle version, SDK, and Java configuration are compatible.
The project has not been independently verified on every Android device or Android Studio version. A successful build and device test should be completed before demonstrating or submitting it.
7. Demonstration Sign-In
The prototype includes demonstration employee credentials:
Email: `manager@smartwood.demo`
Password: `SmartWood123`
These credentials are provided only to demonstrate the prototype interface. The current sign-in is not a secure identity system, and the credentials must not be used for a real company account. If the credentials do not work in the particular project version, check the login logic in the application's JavaScript file.
8. Data Storage and Current Limitations
This project is a prototype. Its current data handling has important limitations:
Most customer and employee data is stored locally using browser storage.
Local data is not automatically synchronised between phones, computers, or users.
Clearing application data or WebView storage may remove saved demonstration records.
The application is not currently connected to a production database or a company server.
Firebase may have been discussed during development, but Firebase is not considered integrated unless the required configuration and working authentication/database code have been added and tested.
The application does not currently receive real-time factory-machine readings or sensor data.
Any production figures, machine statuses, order totals, prices, or reports shown as sample values are not verified live business data.
The employee sign-in is a demonstration feature and should not be used to protect confidential information.
Notification preferences do not mean that a real push-notification service has been configured.
Submitting a customer order or quotation request in the prototype does not guarantee that Sonae Arauco receives it.
Before operational use, the system needs a secure backend, authenticated user accounts, database storage, server-side validation, appropriate access controls, error handling, privacy protections, and full testing.
9. Recommended Future Improvements
Potential improvements include:
Integrate Firebase Authentication or another secure authentication provider.
Connect a database such as Firebase Firestore or a properly designed API-backed database.
Create secure API endpoints for orders, quotation requests, prices, users, production records, and maintenance tasks.
Add role-based access control for customers, employees, supervisors, and administrators.
Synchronise records across devices.
Send order and quotation requests to a monitored business system.
Add genuine push notifications for order updates, alerts, and maintenance reminders.
Connect to authorised production systems or IoT devices for live machine data.
Add server-generated reports with reliable date ranges and export options.
Add automated unit, integration, usability, and security tests.
Validate all form inputs and provide clear error messages.
Review privacy, data retention, backup, and security requirements before deployment.
10. Testing Checklist
Before presenting or submitting the application, test the following on an emulator or physical Android device:
[ ] The project opens and synchronises in Android Studio.
[ ] The application builds and launches successfully.
[ ] The home screen and navigation links work.
[ ] Product information and prices are displayed.
[ ] A customer can complete the order form.
[ ] An order reference and saved order can be looked up.
[ ] A quotation request can be submitted and viewed in the employee area.
[ ] The demonstration employee sign-in behaves as expected.
[ ] Order details and status changes display correctly.
[ ] Price changes behave as expected in the local prototype.
[ ] Production, machine, maintenance, and report screens open.
[ ] CSV export works if available in the selected project version.
[ ] Settings and theme preferences behave as expected.
[ ] The contact information is readable.
[ ] Invalid or incomplete form inputs are handled appropriately.
[ ] The interface remains usable on different screen sizes.
Only mark a test as passed after you have run it and observed the result.
11. GitHub Repository
To publish the source code on GitHub:
Create a new repository on GitHub.
Give it a clear name, such as `smart-wood-production-monitoring-system`.
Add a short repository description explaining that it is an Android prototype for customer orders, quotations, production monitoring, maintenance, and reporting.
Upload the Android project source files and this `README.md`.
Keep `README.md` in the repository's root folder, alongside `settings.gradle`.
Do not upload passwords, API keys, private signing keys, or confidential company information.
If Firebase or another service is integrated later, follow its security guidance and do not publish private credentials.
Check the repository after uploading to ensure that the important source files are visible.
For a team or academic project, follow your lecturer's instructions about repository visibility, commit history, documentation, and source-code submission.
12. Project Status
Status: Prototype / ongoing development
The application demonstrates the intended interface and core navigation for a Smart Wood Production Monitoring System. Some features operate using locally stored demonstration data. It should not be described as a fully deployed, live production system until backend integration, database design, secure authentication, API functionality, and testing have been completed.
13. Disclaimer
This is an educational and demonstration project developed in the context of a Smart Wood Production Monitoring System for Sonae Arauco. It is not an official Sonae Arauco service and is not confirmed to be connected to the organisation's internal systems. Sample records and prices are illustrative only. Confirm all official information and obtain the required authorisation before using the application in a real business environment.
