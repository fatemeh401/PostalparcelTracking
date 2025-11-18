flowchart LR
  %% Actors
  User[User]
  Admin[System Admin]
  Courier[Courier]
  Support[Support Agent]

  %% Use Cases
  UC_LOGIN((Login))
  UC_REGISTER((Register))
  UC_TRACK((Track Shipment))
  UC_VIEW((View Status))
  UC_NOTIFY((Enable Notifications))
  UC_REPORT((Report Issue))

  UC_UPDATE_STATUS((Update Status))
  UC_MANAGE_SHIP((Manage Shipments))
  UC_MANAGE_COURIER((Manage Couriers))
  UC_RESPOND_TICKET((Respond to Tickets))

  UC_SCAN((Scan Package))
  UC_UPDATE_LOC((Update Location))

  %% Relationships
  User --> UC_LOGIN
  User --> UC_REGISTER
  User --> UC_TRACK
  User --> UC_VIEW
  User --> UC_NOTIFY
  User --> UC_REPORT

  Admin --> UC_UPDATE_STATUS
  Admin --> UC_MANAGE_SHIP
  Admin --> UC_MANAGE_COURIER
  Admin --> UC_RESPOND_TICKET

  Courier --> UC_SCAN
  Courier --> UC_UPDATE_LOC

  Support --> UC_RESPOND_TICKET

  %% Styling (optional)
  classDef actor fill:#fff,stroke:#333,stroke-width:2px,font-weight:bold;
  class User,Admin,Courier,Support actor