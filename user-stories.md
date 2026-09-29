```gherkin
User Story: Customer drops off clothes for laundry service.
Scenarios
GIVEN the customer is at the reception
AND the customer has clothes to be washed
WHEN the receptionist records the customer's laundry details
AND the clothes are received
THEN the system should create a laundry order
AND assign the order a unique order number
AND send the clothes to the sorting station.
**User Story:** Customer picks up completed laundry.

GIVEN the customer's clothes have been washed, dried, folded, quality-checked, and packed
AND the laundry order is marked as ready for pickup
WHEN the customer provides the order number
THEN the system should verify the order
AND confirm that the laundry is ready
AND allow the customer to pick up the clothes.

