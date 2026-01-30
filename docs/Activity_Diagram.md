```mermaid
flowchart TD
  Start([Start])
  Login[Login]
  EnterCode[Enter Tracking Code]
  Check{Code Valid?}
  Show[Show Status]
  Error[Error]
  End([End])

  Start --> Login
  Login --> EnterCode
  EnterCode --> Check
  Check -- Yes --> Show
  Check -- No --> Error
  Show --> End
  Error --> EnterCode
```
