# User Stories & Acceptance Criteria: User Management / Authentication

## 1. Sign Up
As aNew User,  
I want to register a new account with my email and password,  
So that I can create a unique identity and access the platform.

### Acceptance Criteria
[1] Valid Email: User must provide a valid email address format (e.g., user@example.com).
[2] Password Strength: Password must be at least 8 characters long and contain at least one number and one special character.
[3] Unique Account: If the email is already registered, show a clear error message: "Account with this email already exists."
[4] Successful Registration: Upon success, the user is created in the database, logged in automatically, and redirected to the "Create or Join Team" page.
[5] Form Validation: "Sign Up" button is disabled until all required fields are filled.

---

## 2. Login
As a Registered User,  
I want to log in with my credentials,  
So that I can securely access my teams and data.

### Acceptance Criteria
[1] Input Fields: Form must accept Email and Password.
[2] Success: Entering valid credentials redirects the user to their Dashboard/Home.
[3] Failure: Entering invalid credentials shows a generic error: "Invalid email or password" (for security).
[4] Session: A secure session token (JWT or cookie) is generated upon login.
[5] Remember Me: (Optional) If "Remember Me" is checked, the session persists after closing the browser.

---

## 3. Logout
As a User,  
I want to log out of the platform,  
So that I can ensure my account is secure when I leave my device.

### Acceptance Criteria
[1] Action: Clicking "Logout" immediately terminates the active session.
[2] Redirect: User is redirected to the Public Landing Page or Login Page.
[3] Security: The session token is invalidated on the server side (if applicable) and removed from the client storage.
[4] Back Button: Clicking the browser's "Back" button after logout does not reveal authenticated pages.

---

## 4. Edit Profile
As a User,  
I want to update my personal information (name, picture, bio),  
So that my team members can easily recognize me.

### Acceptance Criteria
[1] Editable Fields: User can update Display Name, Job Title/Bio, and Profile Picture.
[2] Image Upload: User can upload a standard image format (JPG, PNG) max size 5MB.
[3] Validation: Display Name cannot be empty.
[4] Persistence: Changes are saved immediately and reflected across the UI (e.g., in chat headers).
[5] Cancel: User can cancel edits to revert to previous information without saving.

---

## 5. Role Assignment
As an Admin,  
I want to assign roles (Member / Admin) to users,  
So that I can manage permissions within the team.

### Acceptance Criteria
[1] Access Control: Only users with the "Admin" role can see and use this feature.
[2] Role Selection: Admin can select a user and toggle their role between "Member" and "Admin".
[3] Confirmation: A success toast/notification appears: "User role updated to [Role]."
[4] Self-Lockout Prevention: An Admin cannot remove their own Admin status if they are the *only* Admin.

---

## 6. Delete Account
As a User,  
I want to delete my account,  
So that I can remove my personal data from the platform.

### Acceptance Criteria
[1] Hard Confirmation: User must enter their password or type "DELETE" to confirm the action.
[2] Data Handling: User's personal profile is removed. Their messages/content may be anonymized (e.g., "Deleted User") rather than deleted, to preserve chat history context.
[3] Redirect: User is immediately logged out and redirected to the Homepage.
[4] Email Notification: A "Goodbye" email is sent confirming the account deletion.

---

## 7. Reset Password (Authenticated)
As a User,  
I want to change my current password,  
So that I can keep my account secure.

### Acceptance Criteria
[1] Verification: User must enter their *Current Password* before setting a new one.
[2] New Password Validation: New password must meet the same strength requirements as Sign Up.
[3] Confirmation: User must re-type the new password to confirm.
[4] Success: Upon success, user stays logged in, and a notification "Password updated successfully" is shown.

---

## 8. Forgot Password (Unauthenticated)
As a User,  
I want to request a password reset link,  
So that I can regain access if I forget my credentials.

### Acceptance Criteria
[1] Request: User enters their email address on the "Forgot Password" page.
[2] Email Trigger: If the email exists, a reset link with a time-limited token (e.g., 1 hour) is sent.
[3] Security: The UI shows "If an account exists for this email, a link has been sent" (to prevent email enumeration attacks).
[4] Reset Flow: Clicking the link takes the user to a "Create New Password" page where they can set a new password without knowing the old one.
