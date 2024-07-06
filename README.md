# aws-diagram-ecommerce

**********
Task:
Scenario 1: E-commerce Website
Architecture:
1. Presentation Tier (Frontend):
  - Components:Web browser, Mobile app.
  - Technologies:HTML, CSS, JavaScript, React.js, Swift (for iOS app), Kotlin (for Android app).
2. Application Tier (Backend):
  - Components:Web server, API server.
  - Technologies:Node.js with Express.js, Python with Flask/Django, Java with Spring Boot.
3. Data Tier (Database):
  - Components:Database server.
  - Technologies:MySQL/PostgreSQL (for relational data), MongoDB (for NoSQL data).
Scenario:
An e-commerce website where users browse products, add them to the cart, and complete purchases.
- User Interaction:Users interact with the website or mobile app to search for products, view details, and make purchases.
- Business Logic:The backend server processes product searches, handles user authentication, manages the shopping cart, and processes payments.
- Data Storage: Product information, user accounts, and transaction records are stored in the database.
Flow:
1. The user accesses the e-commerce website or mobile app.
2. The frontend sends requests to the backend to fetch product data.
3. The backend retrieves data from the database and processes it.
4. The backend sends the processed data back to the frontend to display to the user.
5. The user adds products to their cart and proceeds to checkout.
6. The backend processes the payment and updates the transaction data in the database.
**********

Diagram:

![AWS - Scenario 1](https://github.com/njlatonio/aws-diagram-ecommerce/assets/168039404/55158008-1278-4c70-b7f9-1a566b0a482c)

Explanation:
3 regions used to ensure 99.999% availability and to be fault tolerant
- Amazon Route 53 used for DNS services
- Amazon Cloudfront used for edge caching
- Elastic Load balancer used to spread load across availability zones
- Amazon EC2 instances used for web and app servers
- Amazon RDS used for relational databases (MySQL/PostgreSQL)
- Amazon DocumentDB used for MongoDB (NoSQL data)
- Amazon S3 used for static storage and backup
