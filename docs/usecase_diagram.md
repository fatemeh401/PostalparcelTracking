``` mermaid
flowchart LR
  %% Actors
  User[User]
  Admin[System Admin]
  Courier[Courier]
  Support[Support Agent]

  %% Use Cases
  UC_LOGIN((Enter valid email/username & password))
  UC_REGISTER((Provide required information))
  UC_TRACK((Enter valid tracking code))
  UC_VIEW((Show most recent shipment status))
  UC_NOTIFY((Turn notifications on/off))
  UC_REPORT((Choose issue type & enter description))

  UC_UPDATE_STATUS((Select & apply new status))
  UC_MANAGE_SHIP((Edit shipment information))
  UC_MANAGE_COURIER((Edit or deactivate couriers))
  UC_RESPOND_TICKET((Write & submit a response))

  UC_SCAN((Scan package code))
  UC_UPDATE_LOC((Submit new location information))

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

 
