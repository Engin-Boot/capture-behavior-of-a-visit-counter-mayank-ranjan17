# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given the log of patient list and their schedule
  When a patient recovers
  Then the patient leaves the hospital and number of beds vacant count increases by one
  
Scenario: Compute parking slots to reserve for visiting specialists

  Given the parking slot occupancy list by hospital staff
  When a specialist arrives and park his/her vehicle in the reserved parking sport
  Then the Visit-counter increases by one
