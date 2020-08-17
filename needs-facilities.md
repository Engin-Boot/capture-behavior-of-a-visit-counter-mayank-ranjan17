# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given the list of visitors
  When a visitor arrives
  Then the seating arrangement updates by count of one
  
Scenario: Alert when seating capacity is full

  Given the seating capacity
  When there is no vacant place left for a visitor
  Then facility manager put them in the waiting list
