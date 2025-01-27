# lift-management-system
A LLD on managing a passenger lift catering to tall rises


## Requirements
1. The lift moves in two direction. Up and down.
2. It records all the requests to stop from all floors in a central store and decides
   1. Which direction to go (Up or down)
   2. Which floor to stop while moving
3. If it moves in a particluar direction (say up), it should cater all floors in UP direction only sorted in descending order
   1. Eg: If the current floor is 5th and requests looks like this `[(6, down), (7, up), (8, down), (9, up)]`, it should go to 7th -> 9th -> 8th -> 6th
4. The descision making should happen whenever a new request comes in.
