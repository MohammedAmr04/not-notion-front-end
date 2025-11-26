# not-notion-front-end
# Collaborative Team Platform - Use Cases

## 1️⃣ User Management / Authentication

| Use Case | Actor | Scenario | Priority |
|----------|-------|---------|---------|
| Sign Up | New User | User registers a new account with email and password | MVP |
| Login | User | User logs in to access the platform | MVP |
| Logout | User | User logs out of the platform | MVP |
| Edit Profile | User | User updates personal information (name, picture, info) | MVP |
| Role Assignment | Admin | Admin assigns roles to users (Member / Admin) | MVP |
| Delete Account | User | User deletes their account | MVP | add
| Reset Password | User | User resets their password | MVP | add
| Forgot Password | User | User forgot their password | MVP | add

---

## 2️⃣ Teams & Channels

| Use Case | Actor | Scenario | Priority |
|----------|-------|---------|---------|
| Create Team | User | User creates a new team and becomes Admin | MVP |
| Join Team | User | User joins an existing team via invitation link and becomes Member | MVP | edit 
| Mebemer Becomes Admin | User | Admin makes a member an admin | MVP |
| Leave Team | User | User leaves a team | MVP | add 
| Delete Team | User | Admin deletes a team | MVP | add 
| Rename Team | User | Admin renames a team | MVP | add 
| Delete Channel | User | Admin deletes a channel | MVP | add 
| Create Channel | User | Admin or Member creates a new channel within a team | MVP |
| Send Message in Channel | User | User sends a text message in a channel | MVP |
| Invite Member | User | User invites new members to the team via email | MVP |


---

## 3️⃣ Real-Time Collaboration

| Use Case | Actor | Scenario | Priority |
|----------|-------|------------|----------|
| Live Chat | User | As a user, I want to send and receive messages in real-time so I can communicate instantly with my team. | MVP |
| Collaborative Docs | User | As a user, I want to edit documents with others in real-time so we can work together without conflicts. | MVP |
| Whiteboard | User | As a user, I want to draw and brainstorm live with the team so we can collaborate visually. | MVP |
| Real-Time Task Updates | User | As a user, I want task updates to show instantly so everyone sees the most recent project status. | MVP |

---

## 4️⃣ Tasks / Projects Management

| Use Case | Actor | Scenario | Priority |
|----------|-------|---------|---------|
| Create Task | User | User creates a new task within a project | MVP |
| Assign Task | User | User assigns a task to specific members | MVP |
| Update Task Status | User | User changes the status of a task | MVP |
| Rename Task | User | Admin renames a task | MVP | add 
| Comment on Task | User | User adds comments on a task and tracks updates | MVP |
| Delete Task | User | Admin deletes a task | MVP |

---

## 5️⃣ Notifications

| Use Case | Actor | Scenario | Priority |
|----------|-------|---------|---------|
| New Message Alert | User | User receives notification when a new message arrives | MVP |
| New Task Alert | User | User receives notification when a new task is created | MVP | add 
| New Channel Alert | User | User receives notification when a new channel is created | MVP | add 
| New Team Alert | User | User receives notification when a new team is created | MVP | add 
| New Member Alert | User | User receives notification when a new member is added to a team | MVP | add
| Task Update Alert | User | User receives notification when a task is updated or assigned | MVP |
| Doc Update Alert | User | User receives notification when a shared document is updated | MVP |

---

## 6️⃣ Video Calls / Streaming (Phase 2)

| Use Case | Actor | Scenario | Priority |
|----------|-------|---------|---------|
| Video Call | User | User initiates a one-on-one or group video call | Phase 2 |
| Screen Sharing | User | User shares screen during a video call | Phase 2 |
| Call Recording | User | User records the call (optional) | Phase 2 |
| Live Streaming | User | User streams live video to team members | Phase 2 |
| 

---

## 7️⃣ File / Media Sharing (Phase 2)

| Use Case | Actor | Scenario | Priority |
|----------|-------|---------|---------|
| Upload File | User | User uploads a document or file to a channel | Phase 2 |
| Download File | User | User downloads shared files | Phase 2 |
| Access Control | Admin | Admin defines who can upload/download files | Phase 2 |

---

## 8️⃣ AI / Productivity Features (Optional, Phase 3)

| Use Case | Actor | Scenario | Priority |
|----------|-------|---------|---------|
| Auto Summary | User | Generate automatic summaries of chats or meetings | Phase 3 |
| Real-Time Translation | User | Translate messages or documents instantly | Phase 3 |
| Team Analytics | Admin | Analyze team activity and member performance | Phase 3 |

---

> 💡 **Tip:** Focus first on the **MVP**: User Management, Teams & Channels, Real-Time Chat/Docs, Tasks & Notifications.  
> Once the MVP is stable, add Video Calls, File Sharing, and AI features in later phases.
