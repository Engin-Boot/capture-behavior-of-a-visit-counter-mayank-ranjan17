# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given: List of patient with their schedule
  When: When a patient is discharged or attended by a specialist
  Then: The patient's bed is marked as vacant.

Scenario: Compute parking slots to reserve for visiting specialists

  Given: Parking Details of the hospital staffs and visiting specialists
  When: When a specialists visits a hospital 
  Then: The parking spot allocated to the specialists must be empty and "Visit-counter" must be updated by a count of 1.
