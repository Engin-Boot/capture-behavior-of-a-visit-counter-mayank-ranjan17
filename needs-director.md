# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

Given the list of patients with their schedules
When a patient is treated and discharged 
Then the number of beds that are vacant needs to be updated

Scenario: Compute parking slots to reserve for visiting specialists

Given the parking log of hospital staffs
When the specialist arrives and the slot assigned to the specialist is empty
Then the Visit-counter is updated by one
  
  
