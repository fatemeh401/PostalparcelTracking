``` mermaid
flowchart LR
  %% Actors
  User[User]
  Admin[System Admin]
  Courier[Courier]
  Support[Support Agent]

  %% Use Cases
  UC_LOGIN((The user must enter a valid email/username and password.))
  UC_REGISTER((The user must provide required information :email, phone number, password))
  UC_TRACK((The user can enter a valid tracking code.)
  UC_VIEW((VThe system shows the most recent shipment status.))
  UC_NOTIFY((The user can turn notifications on or off))
  UC_REPORT((The user can choose issue type and enter a description.))

  UC_UPDATE_STATUS((he admin can select and apply a new status))
  UC_MANAGE_SHIP((The admin can edit shipment information.)
  UC_MANAGE_COURIER((The admin can edit or deactivate couriers))
  UC_RESPOND_TICKET((The agent can write and submit a response.))

  UC_SCAN((The courier can scan the package code.))
  UC_UPDATE_LOC((The courier can submit new location information.))

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
```

 
