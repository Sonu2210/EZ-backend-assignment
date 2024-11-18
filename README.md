EZ Backend Assignment
  - A secure file-sharing system built with Node.js, MongoDB, and RESTful APIs. This application supports user authentication, file upload/download, and access control to ensure only authorized users can interact with the system.

Features:
  - Users:
      - Operations User (Ops User): Can upload files (.docx, .pptx, .xlsx).
  - Client User:
    Can sign up and verify their email.
    Can view the list of uploaded files.
    Can download files via secure, encrypted URLs.

Technologies Used
- Backend: Node.js, Express.js
- Database: MongoDB with Mongoose ODM
- Authentication: JWT (JSON Web Tokens)
- File Handling: Multer
- Email Service: Nodemailer
- Encryption: Crypto module

How It Works:
1. Sign Up & Verify Email:
   - A Client User signs up via the /auth/signup endpoint.
   - A verification email is sent containing a secure link.
   - The user clicks the link to verify their email.
2. Login:
  - Both Ops and Client Users log in via /auth/login and receive a JWT token.
3. File Upload (Ops User):
  - Ops Users upload files via /files/upload.
  - Only .docx, .pptx, and .xlsx files are allowed.
4. File List & Download (Client User):
  - Client Users can view uploaded files via /files/list-files.
  - Secure, encrypted URLs are generated for downloading files.

Testing the Application:
  - Tools:
      - Postman or curl for API testing.
  - Steps:
      - Test all authentication endpoints (Sign Up, Login, Verify Email).
      - Upload a file as an Ops User.
      - List files and download as a Client User
   
  
