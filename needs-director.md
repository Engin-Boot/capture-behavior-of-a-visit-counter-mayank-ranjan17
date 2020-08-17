# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given the log of patient list and their schedule
  When a patient is treated and discharged
  Then the bed allocated to the patient is marked as vacant
  
Scenario: Compute parking slots to reserve for visiting specialists

  Given the parking slot occupancy list by hospital staff
  When a specialist arrives the slot assigned to the specialist is occupied
  Then the Visit-counter increases by one
