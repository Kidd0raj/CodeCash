# CodeCash
### Backend (Node.js):

#### Framework:
- **Express.js:** A minimal and flexible Node.js web application framework.

#### Data Structures:
1. **User:**
   - `userId`
   - `username`
   - `qrCodes` (array of QR codes associated with the user)

2. **QR Code:**
   - `qrCodeId`
   - `type` (send/receive)
   - `amount`
   - `timeBound` (boolean)
   - `expiryTime`
   - `createdAt`

#### M-Pesa Integration:
- Use Safaricom's Daraja API for M-Pesa integration. You'll need to obtain API keys and follow the documentation provided by Safaricom.

#### Security:
- Implement user authentication using JWT (JSON Web Tokens).
- Use HTTPS to encrypt data in transit.
- Validate and sanitize user inputs to prevent SQL injection and other security vulnerabilities.

#### Testing:
- Use Mocha and Chai for backend unit testing.
- Test key functionalities such as QR code generation, deletion, and M-Pesa integration.

### Frontend (Vue.js):

#### Framework:
- **Vue.js:** A progressive JavaScript framework for building user interfaces.

#### UI Design:
- Create a simple and intuitive UI with Vue.js components for QR code generation, deletion, time-bound QR code, and QR code usage.
- Use a component library like Vuetify for a polished and consistent UI.

#### Security:
- Implement secure communication with the backend using HTTPS.
- Sanitize user inputs to prevent potential security threats.

#### Testing:
- Use Jest and Vue Test Utils for frontend unit testing.
- Test components, especially those related to QR code generation and display.

### Initial SDLC Documentation:

#### Project Overview:
- **Name:** Money Transaction App with QR Code
- **Description:** An application allowing users to generate, delete, and manage QR codes for sending and receiving money, with integration with M-Pesa.

#### Team Members:
- [Ishaq Rajab](rajabmattryn@gmail.com)

#### Technologies Used:
- Backend: Node.js, Express.js, Mocha, Chai
- Frontend: Vue.js, Vuetify, Jest

#### Features:

1. **QR Code Generation:**
   - Users can generate QR codes for sending or receiving money.

2. **QR Code Deletion:**
   - Users can delete QR codes that are no longer needed.

3. **Time-Bound QR Code:**
   - Users can generate QR codes with a specified expiration time.

4. **Active QR Codes:**
   - Users can view a list of active QR codes associated with their account.

5. **QR Code Usage:**
   - Users can view the usage history of a particular QR code.

#### SDLC Phases:

1. **Planning:**
   - Define project scope, objectives, and requirements.
   - Identify team members and assign roles.

2. **Design:**
   - Create data models for users and QR codes.
   - Design the UI components and user flows.
   - Plan M-Pesa integration.

3. **Implementation:**
   - Set up the Node.js backend with Express.js.
   - Implement user authentication and authorization.
   - Develop QR code generation, deletion, and M-Pesa integration.
   - Set up the Vue.js frontend with necessary components.

4. **Testing:**
   - Conduct unit tests for both backend and frontend.
   - Perform integration testing for QR code generation and M-Pesa integration.

5. **Deployment:**
   - Deploy the application on a hosting platform.
   - Configure environment variables.

6. **Monitoring and Maintenance:**
   - Implement monitoring for application health.
   - Provide documentation for maintenance tasks.

This initial SDLC documentation provides a high-level overview of the project, its features, and the technologies used. As the project progresses, I will expand and refine this documentation with more detailed information
