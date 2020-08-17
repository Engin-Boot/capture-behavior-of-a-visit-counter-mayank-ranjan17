# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given the server recovers
  When the server restarts
  Then the visit counter resets to the number of visits as detect by the sensor

Scenario: Reconcile counts if the sensor is offline for a while

  Given the sensor restarts
  When the sensor is online again
  Then the sensor needs to perform the total count again
