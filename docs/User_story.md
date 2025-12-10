#  User Stories & Acceptance Criteria
Shipment Tracking System  
---

## 1. Login
### User Story
As a user, I want to log into the system so that I can access my shipment information.

### Acceptance Criteria
- The user must enter a valid email/username and password.
- An error message is shown if credentials are incorrect.
- On successful login, the user is redirected to the dashboard.

---

## 2. Register
### User Story
As a new user, I want to create an account so that I can track my shipments.

### Acceptance Criteria
- The user must provide required information (email, phone number, password).
- The system validates uniqueness of email/phone number.
- A confirmation message is displayed after successful registration.

---

## 3. Track Shipment
### User Story
As a user, I want to enter a tracking code so that I can follow my shipment.

### Acceptance Criteria
- The user can enter a valid tracking code.
- The system displays the shipment’s current status and history.
- Invalid codes show an appropriate error message.

---

## 4. View Shipment Status
### User Story
As a user, I want to view the real-time status of my shipment so that I know its current location.

### Acceptance Criteria
- The system shows the most recent shipment status.
- Status includes timestamp, location, and event type.
- The page must load without errors.

---

## 5. Enable Notifications
### User Story
As a user, I want to enable notifications so that I am informed of shipment updates.

### Acceptance Criteria
- The user can turn notifications on or off.
- The system sends alerts when the shipment status changes.
- Notifications must be delivered to the user's device.

---

## 6. Report Issue
### User Story
As a user, I want to report an issue so that the support team can review and resolve it.

### Acceptance Criteria
- The user can choose issue type and enter a description.
- The system creates a ticket with a tracking ID.
- A confirmation message is shown to the user.

---

# Admin Use Cases

## 7. Update Shipment Status
### User Story
As an admin, I want to update shipment statuses so that users can view the latest information.

### Acceptance Criteria
- The admin can select and apply a new status.
- Status updates are saved and visible to users.
- Users receive notifications if enabled.

---

## 8. Manage Shipments
### User Story
As an admin, I want to manage shipments so that I can maintain accurate operational data.

### Acceptance Criteria
- The admin can create new shipments.
- The admin can edit shipment information.
- The system shows a searchable shipment list.

---

## 9. Manage Couriers
### User Story
As an admin, I want to manage couriers so that delivery operations remain organized.

### Acceptance Criteria
- The admin can add new couriers.
- The admin can edit or deactivate couriers.
- The system displays each courier’s current status.

---

# Support & Admin

## 10. Respond to Tickets
### User Story
As a support agent or admin, I want to respond to tickets so that user issues can be resolved.

### Acceptance Criteria
- Tickets are listed and can be filtered.
- The agent can write and submit a response.
- Users receive a notification when their ticket is answered.

---

#  Courier Use Cases

## 11. Scan Package
### User Story
As a courier, I want to scan packages so that each process step is recorded.

### Acceptance Criteria
- The courier can scan the package code.
- The system records scan time and location.
- Invalid codes show an error message.

---

## 12. Update Location
### User Story
As a courier, I want to update the location so that shipment tracking remains accurate.

### Acceptance Criteria
- The courier can submit new location information.
- The system stores coordinates and timestamp.
- Updated information is visible to users.

---

# End of Document
