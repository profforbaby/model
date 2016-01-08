This readme file explains the format of the instances using file demo-instance.xml as an example.

Assumptions

- We have a total of 1 device of type 1 available at the start of the planning
- We have a total of 3 devices of type 2 available at the start of the planning
- A device of type 1 weights 8 units
- A device of type 2 weights 8 units
- There is one type of vehicle per driver
- There are two drivers and two vehicle types
- Each vehicle type has one vehicle and one unique driver
- A vehicle can carry up to 150 or 80 units of weight
- There are 6 customers, one depot and two driver start locations
- Nodes with type=2 are the customers and the node with type=0 is the depot (end location) and with type=1 a start location
- A vehicle start at its driver start location and ends their route at the depot
- A driver has a time-window in which he must start at his start location and end at the depot
- The underlying graph is complete and asymmetric
- Requests with type=0 represent device pick-up request and with type=1 device deliver request.
- Requests that do not involve picking up or delivering devices have type=2
- Request with priority of 1 are considered to have maximum priority
- Request with priority of 2 are considered to have minimum priority

- Customer 1 needs us to pickup 2 devices of type 1 with high priority (=1), which takes 360 time units of service time
- Customer 2 needs us to deliver 1 devices of type 2 with high priority (=1), which takes 120 time units of service time
- Customer 3 needs us to visit with high priority (=1), which takes 180 time units of service time
- Customer 4 needs us to deliver 2 devices of type 1 with low priority (=0), which takes 240 time units of service time
- Customer 5 needs us to pickup 3 devices of type 2 with high priority (=1), which takes 540 time units of service time
- Customer 6 needs us to visit with low priority (=0), which takes 180 time units of service time